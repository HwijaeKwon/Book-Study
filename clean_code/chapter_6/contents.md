# Objects and Data Structures
## Data Abstraction
## Data/Object Anti-Symmetry
- object: hide their data behind abstractions and expose functions that operate on that data
- data structure : expose their data and have no meaningful functions
- Procedual code (code using data structures) makes it easy to add new functions without changing the existing data structures.
- OO code, on the other hand, makes it easy to add new classes without changing existing functions.

## The Law of Demeter
- A module should not know about the innards of the objects it manipulates.

## Active Record
- Unfortunately we often find that developers try to treat these data strucutures as though they were objects by putting business rule methods in them. (Sorry...)
- The solution, of course, is to treat the Action Record as a data structure and to create seperate objects that contain the business rules and that hide their internal data.

## Conclusion
- Object : expose behavior and hide data
  - easy to add new kinds of objects without changing existing behaviors
  - hard to add new behaviors to existing objects
- Data structure : expose data and have no significant behavior
  - easy to add new behaviors to existing data structures
  - hard to add new data strucutures to existing functions
- Flexibility!!!
- Good software developers understand these issues without prejudice and choose the approach that is best for the job at hand.
