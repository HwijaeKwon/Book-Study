# Formatting
## The Purpose of Formatting
- Code formatting is about communication, and communication is the professional developer's first order of business.

## The Newspaper Metaphor
- Top down
- name : should be sufficient to tell us whether we are in the right module or not
- topmost parts : provide the high-level concepts and algorithms
- details : increase as we move downward

## Vertical Openness Between Concepts
- Blank lines : visual cue that identifies a new and seperate concept

## Vertical Density
- close association : lines of code that are tightly related should appear vertically dense

## Vertical Distance
- concepts that are closely related should be kept vertically close to each other (doesn't work for concepts that belong in seperate files)
- closely related concepts should not be seperated into different files unless you have a very good reason.
- vertical seperation should be a measure of how important each is to the understandability of the other.
### Variable Declarations
- Variables should be declared as close to their usage as possible.
- Instance variables should be declared at the top of the class.
### Dependent Functions
- If one function calls another, they should be vertically close and the caller should be above the callee, if at all possible.
### Conceptual Affinity
- The stronger that affinity, the less vertical distance there should be between them.
### Vertical Ordering

### Horizontal Formatting
- Strive to keep our lines short (< 120)

### Horizontal Openness and Density
### Horizontal Alignment

### Indentation
#### Breaking Indentation

## Team Rules
## Uncle Bob's Formatting Rules
