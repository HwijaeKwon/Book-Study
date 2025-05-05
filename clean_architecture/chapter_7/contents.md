# Design Principles (SOLID)
- The goal of the principles is the creation of mid-level(module level) software structures that
  - Tolerate change
  - Are easy to understand
  - Are the basis of components that can be ued in many software systems.  
- SRP : The Single Responsibility Principle
- OCP : The Open-Closed Principle
- LSP : The Liskov Substitution Principle
- ISP : The Interface Segregation Principle
- DIP : The Dependency Inversion Principle

# SRP : The Single Responsibility Principle
- A module should have one, and only one, reason to chage = A module should be responsible to one, and only one, *actor*
  - actor : one or more people who require that change (ex. user, stakeholder, ...)
  - module : source file, cohesive set of functions and data structures.

## Symptom 1 : Accidental Duplication
## Symptom 2 : Merges
- Seperate the code that different actors depend on.

## Solutions
- Seperate data from the functions
- Seperate functions into individual classes + Facade pattern
