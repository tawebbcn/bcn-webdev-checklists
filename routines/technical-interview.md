TECHNICAL INTERVIEW

# INTRODUCTION
- Ironhack is selling a product for people with no previous JS skills
- The purpose of the technical interview is to evaluate basic logic skills by asking for simple abstraction concepts
- The TI will last 45 minutes (basic exercises) but will be extendable to 60 minutes (bonus exercise)
- After every TI, the TA will show the applicant what is Codewars
- All the steps in this guide are subject to change depending on each particular case and the TA's and Admissions Manager's criteria

# GUIDELINE

## STARTING
- Get basic information from the applicant and explain how the TI works. e.g.:
  - What is your motivation for doing the bootcamp?
  - Do you have previous coding experience?
  - We don't evaluate your JS skills
  - We evaluate your logical reasoning
  - Always ask what are you thinking
  - Ask for doubts about the TI

## DURING
- Present the exercises by order, starting from 0
- If the applicant doesn't solve at least exercise 2, he/she does not pass the technical interview
- If the current interview is a second opportunity, he/she must solve the hard version until exercise 3
- If the applicant solves the exercises easily, he/she can skip to the bonus exercises or try to solve the hard versions

## ENDING
- The TA will send the feedback to the Admissions Manager and he/she will send you the next steps
- We don't decide if you are accepted or not
- Show Codewars to the applicant as a suggestion to start coding

### IF APPLICANT ASKS WHY ANGULAR (INSTEAD OF REACT)
- Explain that Angular is a complete framework and perfect to show and explain the concept of a single page application in one week. React is a library and together with it, students would need to learn, React Router and Redux which wouldn't be realistic to cover in just one week.

## FEEDBACK TO ADMISSIONS
- Use feedback template:
  - pass technical interview: yes | no
  - previous experience: yes | no
  - logic: low | basic | good
  - expected bootcamp experience: hard | medium | ready
  - recommend second opportunity: yes | no
  - comment: why this recommendation

# EXERCISES

## EXERCISE 0 - CREATE ARRAY
- Purpose of the exercise: 
  - test JS level
- Before starting:
  - What is an array?
  - How to access an element?
  - How to know the length?
- If he/she doesn't know: 
    - an array is a data structure that contains a group of elements where you can access any element of it
    - .length method
    - access to an element of the array with [index]
    - index starts at 0
- Description, example of practical case:
  - Imagine there is a list with the maximum temperature per day. Represent all the temperatures in an array and give us how many temperatures are and the first temperature of the array
- If he/she doesn't know how to solve it: 
  - write for them and explain it

## EXERCISE 1 - PRINT ALL THE ARRAY
- Purpose of the exercise: 
  - test basic loop abstraction
- Before starting:
  - What is a loop?
  - What is a `for` loop?
- If he/she doesn't know: 
  - explain `for` loops logic and syntax @todo
- Description, example of practical case: 
  - now I want to see every temperature.
- If he/she doesn't know how to solve the problem: 
  - `for` loop example with index to see how it increases
- If still doesn't know how to solve the problem: 
  - does not pass the technical interview

## EXERCISE 2 - (MEDIUM) PRINT FOR EACH DAY IF TEMP IS ABOVE 30 | (HARD) PRINT IF IT'S ODD/EVEN
**IF THE APPLICANT SOLVES THIS EXERCISE, PASSES THE TECHNICAL INTERVIEW**
- Purpose of the exercise: test basic conditional abstraction
- Before starting:
  - What is condition (control structure)?
  - What is `if` statement?
- If he/she doesn't know: 
  - logic `if` statement explanation and syntax @todo
- Description, example of practical case: 
  - I want to know for each day if the temperature is above 30
- If he/she doesn't know how to solve the problem: 
  - if statement example with one number
- If still doesn't know how to solve the problem: 
  - does not pass the technical interview

## EXERCISE 3: BONUS 1 - (MEDIUM) PRINT TEMPERATURE AVERAGE | (HARD) MIN/MAX @todo
- Purpose of exercise: 
  - test scope abstraction (overwrite a variable)
- Before starting:
  - Delete everything but array
  - How to do the average? (logic)
  - If he/she doesn't know: 
    - explain what is average and let him/her start only with the total sum of array
- Description, example of practical case: 
  - I want to know the average temperature
- If he/she doesn't know how to solve the problem: 
  - write the variable `sum` outside the `for` loop
- If still doesn't know how to solve the problem: 
  - solve it and explain it

## EXERCISE 4: BONUS 2 - RECURSIVE OR COMPLEX PROBLEM
- Purpose of the exercise: have fun
- Before starting: 
  - what does he/she want to do? Infinite discount, Factorial, Fibonacci
- If he/she doesn't know: 
  - explain every problem and let them choose
- Description, example of practical case:
  - Infinite discount (easy): given a number, apply a 1% discount and display it every time while the number is bigger than one
  - Factorial (medium): given a number N, multiply this number by the following ones in descendant order until 1 | e.g. 3! = 3 * 2 * 1
  - Fibonacci (hard): series of numbers. The next number is the sum of the 2 before
    given a number N, return the N first Fibonacci series | e.g. F(8) = 1,1,2,3,5,8,13,21
- If he/she doesn't know how to solve the problem: 
  - solve with him/her, pair programming
## SEBA EXERCISES:
```
// Exercise 1. Define an array of 6 positive numbers lower than 50. Called it temperatures. They dont need to be in any specific order.
var temperatures = [45, 32, 2, 8, 12, 27]


// Exercise 2. Print on terminal the length of the temperatures array using the following format "temperatures length -> 6"
console.log("temperatures length -> " + temperatures.length)


// Exercise 3. Print on the terminal all the elements of the array, one by one
for (var ix = 0; ix < temperatures.length; ix++) {
  console.log(temperatures[ix])
}


// Exercise 4. Print on the terminal only the elements of the array that are lower than 25. For the elements that are greater or equal than 25 print "too hot".
for (var ix = 0; ix < temperatures.length; ix++) {
  if (temperatures[ix] < 25) {
    console.log(temperatures[ix])
  } else {
    console.log("too hot")
  }
}


// Bonus. Print on the terminal the average temperature of the temperatures array.
var sum = 0;
for (var ix = 0; ix < temperatures.length; ix++) {
  sum += temperatures[ix];
}
console.log(sum / temperatures.length);

var sum = temperatures.reduce(function(acum, current) {
  return acum + current
}, 0)
console.log(sum / temperatures.length);


// Extra Bonus. Implements a fizzBuzz(num) function that prints the numbers from 1 to num. If it’s a multiple of 3, it should print “Fizz”. If it’s a multiple of 5, it should print “Buzz”. If it’s a multiple of 3 and 5, it should print “Fizz Buzz”.

function fizzBuzz(num) {
  for (var ix = 1; ix <= num; ix++) {
    if (ix % 3 === 0 && ix % 5 === 0) {
      console.log('FizzBuzz')
    } else if (ix % 3 === 0) {
      console.log('Fizz')
    } else if (ix % 5 === 0) {
      console.log('Buzz')
    } else {
      console.log(ix)
    }
  }
}

fizzBuzz(20)
```
# RESOURCES
  - [Codewars](https://codewars.com)
  - [Online Editor](https://www.skype.com/en/interviews/)
  - [Pipedrive](https://ironhack.pipedrive.com/pipeline/1/filter/1)
  - Snippets for BONUS 2 @todo
