# Module 3

# Week 7

> ## Day 1

### Retrospective (2hs) (9.30 to 11.30)
  - [Retro - checklist](https://github.com/ironhack/webdev-checklists/tree/master/retrospectives)

### Break (15min) (11.30 to 11.45) 

### Research (30min) (11.45 to 12.15)
  - typescript
  - dynamic typed vs static typed languages

### Research review (45min) (12.15 to 13.00) 15

### Lunch (1h) (13.00 to 14.00)

### Typescript (30min) (14.00 to 14.30)
  - introduccion
    - created by microsoft
    - open source
    - superset of javascript
    - static typing
    - modules, namespaces and strong OOP support
    - compilation step (catch errors)
  - installation
    - `npm install -g typescript`
    - type `tsc` in the terminal to check installation
  - compilation
    - type `tsc name-of-the-file.ts` to compile
    - file extension .ts > .js
  - features
    - types
      - file extension .ts > .js
      - `let myVarName: dataType = value;`
      - `let myNumber:   number  = 42;`
        `let myBoolean:  boolean = true;`
        `let myString:   string  = "Hello World";`
        `let unusable:   void    = undefined; // Used for functions which don't return a value.`
        `let myWhatever: any     = { hello: 'World' }; // Can be any other type`
    - generics
      - JavaScript arrays are an example of a generic type because they can hold elements of any type
      - `let myArray: Array<T> = [];`
      - `let myArray: Array<string> = ['a','b','c']; // Array of strings`
      - `let myArray: Array<number> = [1, 2, 3]; // Array of numbers`
    - interfaces
      - are like an abstract class (you cannot create objects out of an interface, classes can implement an interface)
    - classes
    - decorators
      - A Decorator is an object-oriented pattern that adds behaviour to classes and methods
      - A decorator is just a function that is going to decorate (populate) a target.

  - resources
    - [TypeScript - JavaScript that scales.](https://www.typescriptlang.org)
    - [What is TypeScript and why would I use it in place of JavaScript? - Stack Overflow](https://stackoverflow.com/questions/12694530/what-is-typescript-and-why-would-i-use-it-in-place-of-javascript/35048303#35048303)

### Break (10min) (14.30 to 14.40)

### Hello Angular 2 (1h) (14.40 to 15.40)
  - client-server arquitecture
  - backend rendered vs frontend rendered
  - SPA (single page applications)
  - Angularjs vs Angular 2+
  - resources:
    - [Angular Docs](https://angular.io/)

### Break (5min) (15.40 to 15.45)

### Mob website from BE render to FE render - Quick demo (2h 15min) (15.45 to 18.00)
  - mob website
    - we will expose events (response as json)
    - create an angular app to render events in the frontend
  - thing to show during the live code:
    - backend setup (postman)
    - app initialization
    - tipical angular arquitecture
    - how to initialize services, pages and components
    - modules
    - event service & httpClient
    - dependency injection
    - components
    - ngIf (loading pattern), ngFor (list of cards)

### Daily exercise
  - as we dont give today the component lecture they are wont be able to do the angular daily, an option is to give the typescript PP exercise as daily
  - [GitHub - ironhack-labs/lab-typescript](https://github.com/ironhack-labs/lab-typescript)

### Research: SPA frameworks (history) & RestAPI
  - SPA frameworks (history)
  - RestAPI
  
## Day 2

### Review: SPA frameworks (history) & RestAPI

### Angular components (2hs) (9.30 to 11.30)
  - install CLI `npm install -g @angular/cli`
  - ng new, ng generate & ng serve
  - tipical angular arquitecture (building blocks)
    - components & pages
    - services
    - pipes
  - components introduction:
    - life cycle hooks (constructor, ngOnInit, ngOnchanges, ngOnDestroy)
    - component structure (encapsulated MVC)
    - how to render a component on a template
    - nested components

### Break (10min) (11.30 to 11.40)

### Angular modules and ngModule (1h 20min) (11.40 to 13.00)
  - modules in ESM
    - module declaration (with export)
    - module import
  - ngModule
    - explain how modules work in angular
    - how to import a ngModule
    - appModule

### Lunch (1h) (13.00 to 14.00)

### Angular data binding (1hs 40min) (14.00 to 15.40)
  - interpolation `{{}}`
  - property binding `[]` (data flow from logic layer to the template)
  - event binding `()` (data flow from template to logic layer)
  - to ways data binding `[()]` (data flow in the two ways) (requires forms module)
  - template variables `#`

### Break (10min) (15.40 to 15.50)

### Activity: Components(40min) (15.50 to 16.30)
  - MVC with the 3 parts of the components
  - explain in the templates {{}}, [], (), [()]

### Review: Group activity (30min) (16.30 to 17.00)

### Angular directives (1h) (17.00 to 18.00)
  - what are directives
  - ngIf (to display or hide)
  - ngFor (to iterate)
  - ngSwitch (when you have several case for many conditions)
  - ngClass (to dynamically apply css classes)
  - ngStyle (to set css property to an element)

### Research: Services & Ajax in angular

### Daily exercise
  - [GitHub - ironhack-labs/lab-ironcontacts](https://github.com/ironhack-labs/lab-ironacontacts)


## Day 3 (Slow demo)
  - all day combining research + demo + mobbing with the students
  - note: dont try this at home

### Review: Services & Ajax in angular (30min)

### Create another app
  - same backend
  - api route
  - instagram clone (images)

### Services (1h 30min)
  - why we use services
    - dry / abstraction (talking to API)
    - sharing state between components
  - using services
  - service injection
  - multiple instance vs singleton
  - dependecy injection
  - httpClient

### Break (10min)

### Routing (1h 50min)
  - angular router
  - setting up routes
  - router outlet
  - RouterLink
  - route parameters
  - router navigate
  - 
### Lunch (1h)

### Rest API Express (1h 50min)
  - REST Overview
  - Setup an API (express)
  - http mehods
  - postman
  - CORS!!!!

### Break (10min)

### HTTP (1h 30min) 
  - HttpModule
  - http in services
  - observables in http
  - we use promises

### Daily exercise
  - find other exercise
  - [GitHub - ironhack-labs/lab-angular-cinema-billboard](https://github.com/ironhack-labs/lab-angular-cinema-billboard)

## Day 4

### RestAPI - Planning (30min)
  - planning
  - setting up server
  - setting up models
  - setting up routes
  - test routes in postman

### Mob programming - RestAPI (3hs)

### Lunch (1h) (13.00 to 14.00)
  
### SPA Frontend - Planning (30min)
  - setting up client
  - generate components
  - generate services

### Mob programming - SPA (3hs)

### Daily exercise - Weekend
  - add api route to the mob website backend
  - Mob website mobile apps

### Research: Pipes
  - Add a date pipe in the daily exercise





## Day 5 (Tunathon)

## Parking lot

## Day 1 (week 2)

### Forms (1h 30min)
  - forms module
  - input validation

### Component I/O (1h 30min) (11.10 to 12.30)
  - component interaction
  - input
  - output
  - 
### Activity: Components I/O (30min) (12.30 to 13.00)
  - `app-card [item] (delete)`
  - 
### Authentication (2hs) (9.30 to 11.30)
  - setting up the backend
  - test in postman
  - setting up the client
    - components nedded
    - auth service

### Break (15min) (11.30 to 11.45)

### Route guards (1h 15min) (11.45 to 13.00)
  - canActivate
  - canDeactivate

### Lunch (1h) (13.00 to 14.00)

### Project kickoff (1h 15min) (11.45 to 13.00)



### Deployment
### File upload
### Maps
