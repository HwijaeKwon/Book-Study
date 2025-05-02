# Functions
## Small
- Functions should be small.

## Blocks and indenting
- Blocks within if, else, while, and so on statements should be one line long.
  - In block -> one function with nice name
 
## Do One Thing 
- Functions should do one thing. They should do it well. They should do it only.
- How to define one thing?
  - If a function does only those steps that are one level below the stated name of the function, then the function is doing one thing.
  - A function is doing more than one thing if you can extract another function from it with a name that is not merely a restatement of its implementation.

## One Level of Abstraction per Function
- Statements within one function are all the same level of abstraction.
- Mixing levels of abstraction within a function is always confusing.

## Reading Code from Top to Bottom: The Stepdown Rule
- We want the code to read like a top-down narrative.

## Switch Statements
- Swith statemetns -> Large. Hard to do one thing.
- We can't always avoid switch statements, but we can make sure that each switch statment is buried in a low-level class and is never repeated.
- Switch statements can be tolerated if they appear only once, are used to create polymorphic objects, and are hidden behind an inheritance.

## Use Descriptive Names
- Choose good names for small functions that do one thing.
- Don't be afraid to make a name long.
  - A long descriptive name is better than a short enigmatic name.
  - A long descriptive name is better than a long descriptive comment.
- Don't be afraid to spend time choosing a name.

## Function Arguments
- Reducing the number of arguments.
  - Arguments at a different level of abstraction force you to know a detail.
  - Hard to test.
### Common Monadic Forms
- 1. Asking about that arguments, 2. Transforming it into something else and returning it -> Naming is important
- Event -> there is an input argument but no output argument. -> Name and contexts
- Don't follow these forms.
  - Using an output argument instead of a return value for a transformation is confusing.
    - ```
      1. StringBuffer transform(StringBuffer in)
      2. void transform(StringBuffer out)
      1 is better than 2
      ```
### Flag Arguments
- Flag arguments are ugly. -> function does more than one thing. (true / false)

### Dyadic Functions
### Triads
- Think very carefully before creating a triad.

### Argument Objects
### Argument Lists
### Verbs and Keywords
- Encode the names of the arguments into the function name.
- ex. assertEquals -> assertExpectedEqualsActual

## Have No Side Effects
- If the function do one thing, there is no side effects.
- Side effects means there are other hidden things that the function do.

## Output Arguments
- In general, output arguments should be avoided.
- If your function must change the state of something, have it  change the state of its owning object using OO.

## Command Query Separation
- Functions should either do something or answer something.

## Prefer Exceptions to Returning Error Codes
- Returning error codes from command functions is a subtle violation of command query seperation.
### Extract Try/Catch Blocks
- It is better to extract the bodies of the try and catch blocks out into functions of their own.
### Error Handling Is One Thing
- Functions should do one thing. Error handling is one thing.
### The Error.java Dependency Magnet
- Use exceptions rather than error codes.

## Don't Repeat Yourself

## Structured Programming
- One entry, one exit.
- If you keep your functions small, then the occasional multiple return, break, or continue statement does no harm and can sometimes even be more expressive than the single entry, single exit rule.
- goto only makes sense in large functions.

## How do you write functions like this?
- Step by step.
- Message, refine, split, rename, eliminate duplication, test code

