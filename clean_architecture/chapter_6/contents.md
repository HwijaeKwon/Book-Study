# Functional Programming
- Variables in functional languages do not vary.

## Immutability And Architecture
- All race conditions, deadlock conditions, and concurrent update problems are due to mutable variables.
- The question you must be asking yourself, then, is whether immutability is practicable.

## Segregation of mutability
- Segregate the application, or services into mutable and immutable components.
  - immutable -> purely functional / communicate with other components that are not purely functional.
- Push as much processing as possible into the immutable components.
- Drive as much code as possible out of those components that must allow mutation.

## Event Sourcing
- The more memory we have, and the faster our machines are, the less we need mutable state.
- We store the transactions, but not the state for the reasonable lifetime of the application.
- CRUD -> CR
