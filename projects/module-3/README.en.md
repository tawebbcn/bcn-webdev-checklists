# Project Name

- Description

## User Stories

  **404:** As an anon/user I can see a 404 page if I try to reach a page that does not exist so that I know it's my fault
  
  **Signup:** As an anon I can sign up in the platform so that I can start saving favorite restaurants
  
  **Login:** As a user I can login to the platform so that I can see my favorite restaurants
  
  **Logout:** As a user I can logout from the platform so no one else can use it 

  **List Restaurants** As a user I want to see the restaurants so that I can choose one to eat
 
  **Add to favorites** As a user I want to add a restaurant to favorite so that I can save the restaurants that I liked the most

  **See my favorites** As a user I want to see my favorite restaurantes so that I can see the ones I liked the most

## Backlog

  **Profile:** As a user I would like to see other users profile so I can see which restaurants they favored

  **Google Maps:** As a user I want to see a map so that I can choose a restaurant nearby
  
# Client

## Routes

  - / - Homepage
  - /auth/signup - Signup form
  - /auth/login - Login form
  - /restaurants - restaurant list
  - /restaurants/:id - restaurant detail
  - /profile/me - my details and favorite restaurants

  ### Backlog

  - /profile/:id

## Services

- Auth Service
  - auth.login(user)
  - auth.signup(user)
  - auth.logout()
  - auth.me()
- Profile Service
  - profile.me()
- Restaurants Service
  - restaurants.list()
  - restaurant.detail(id)   

## Pages

- 404 Page
- Sign in Page
- Log in Page
- Home Page
- Restaurants List Page
- Restaurant Detail Page
- My Profile Page

## Components

- Navbar component
- Restaurant Card component
- Login/Signup form component

## IO

- Restaurants List Page inputs restaurante Restaurant Card component: Display all restaurants in a grid
- Login/Sign up form outputs the form to the parent component

## Guards

- if logged in cannot access login/signup page
- if not logged in cannot access profile page
- if not logged in cannot access history page

# Server

## Models

  User model

  ```
  username - String // required
  email - String // required & unique
  password - // required
  ```

  Restaurant model

  ```
  name - String // required
  email - String // required & unique
  phone - String
  address - String
```

## API Endpoints/Backend Routes

  - GET /auth/me
  - POST /auth/signup
  - POST /auth/login
  - POST /auth/me
  - GET /profile/me
  - POST /favorite
  - GET /restaurante
  - GET /restaurant/:id
  
  
