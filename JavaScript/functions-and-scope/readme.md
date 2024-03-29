# Lecture Reference: Functions and Scope ###################

    # crowdsourced answers:
        # block of code
        # gives actions
        # returns a value 
        # takes input, returns output
        # helps you not repeat yourself
        # can be reused/invoked again
        # abstraction --> making general rather than specific
        # declaration --> when you define a function
        # invocation --> when you call function, aka tell it to run
    # ELI5 (explain like I'm 5)
        # a set of specific actions you can reuse many times
        # like training a dog to do a command. giving command is calling the function
        # flip lightswitch --> light goes on
        # mathematic functions 
        
# How do we declare a function? #################
## Option 1: Named Function Declaration
```js
function addTwoPlusOne() {
    return 2 + 1
}
```

## Option 2: Function Expression
- This is when you save a function to a variable
- We say JS functions are *first-class objects* because you can:
  1. Save functions to variables 
  2. Return a function from another function

```js
const doSomething = function() {
    return "hi"
}
```

## Option 3: Arrow Function
- Just a more compact way of writing a function expression
- Can be written on one or multiple lines
- If no curly braces, *must* use `return` keyword
- Most often used in callbacks, e.g. in an ```array.map()```)

### Single-line arrow function
- Has implicit return; no need to use `return` keyword
```js
const doSomethingArrow = () => "hi" 
```
                # the first equals sign is still assignment operator
                # the parentheses are still a holder for parameter(s)
                # parens optional if only one parameter
                # differences: function keyword omitted; arrow symbol after parentheses

        const doSomethingArrowMultipleLines = () => {
            return "hi" # <-- if function is written across multiple lines,
                        # there's no implicit return so you must use return keyword
        }     

# Other options
- tktk add link tktk     

# How do we call a function?
    addThree(5)

# What are function parameters?
    # placeholders for what you'll pass in to the function
    # what goes in the parentheses
    # here, parameter is num:
        const addThree = (num) => {
            return num + 3
        }


# What are arguments?
    # what you pass into the function when you call it
    # align with the parameters you indicate in the declaration
    # like a plug being plugged into a socket
    # below, we're calling addThreeNums() with the arguments 6, 3, and 1:

    function addThreeNums(num1, num2, num3) {
        return num1 + num2 + num3
    }

    addThreeNums(6, 3, 1)

# What is Scope?
    # where any given variable is accessible in the program

    # Global scope
        # variables declared at top level of your file 
        # (that is, not inside a function or block)
        # can be accessed in all functions and blocks

    # Function/local scope 
        # variables declared inside a function
        # can be accessed only inside that function, and within any blocks inside of it

    # Block scope?
        # variables declared inside a block, such as a loop or conditional
        # can only be accessed inside that one block

# What is a callback function?
    # a function that gets called by another function

# What is a higher-order function?
    # a function that calls another function

# What’s the difference between referencing a function and invoking a function?
    console.log("referenced:" + " " + doSomething)
    console.log("invoked:" + " " + doSomething())

