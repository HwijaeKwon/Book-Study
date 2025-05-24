# Independence
- Good architecture must support
  - the use case and operation of the system
  - the maintenance of the system
  - the development of the system
  - the deployment of the system
 
## Use cases
- Architetures of the system must support the intent of the system.

## Operation
## Development
- Conway's law
  - Any organization that design a system will produce a design whose structure is a copy of the organization's communication strucuture.
 
## Deployment
- The goal is 'immediate deployment'
- A good architecture helps the system to be immediately deployable after build
- This is achieved through the proper partitioning and isolation of the components of the system.
  - master components that tie the whole system together and ensure that each component is properly started, integrated, and supervised.

## Leaving Options Open
- A good architecture balances all of these concerns with a component structure that mutually satisfies them all. -> Pretty hard

## Decoupling Layers
- Single Responsibility Principle and Common Closure Principle -> seperate thoses things that change for different reasons, and to collect those things that change for the same reasons.
- ex. system divided into decoupled horizontal layers - UI, application-specific business rules, application-independent business rules, and the database

## Decoupling Use cases
- Use cases are narrow vertical slices taht cut through the horizontal layers of the system.

## Decoupling Mode
- The decoupling that we did for the sake of the use cases also helps with operations
- We have to seperate our components all the way to the srevice level.
- A good architecture leaves options open -> the decoupling mode is one of the options

## Independent Developability
## Independent Deployability

## Duplication
- True duplication : every change to one instance necessitates the same change to every duplicate of that instance
- False or accidental duplication : evolve along different paths (differenct rates, different reasons)
- Make sure the duplication is real.

## Decoupling Modes (Again)
- Source level : Changes to one module do not force change or recompliation of others
  - same address spaces
  - communicate each other using simple function calls
  - monolithic structure
- Deployment level : changes to the source code in one module do not force others to be rebuilt and redeployed
  - some of them lives in the same address, communicate through functions
  - others live in other processes in the same processors, and communicate through interprocess communications, sockets, or shared memory.
 - Service level : reduce the dependencies down to the level of data structures, and communicate soley through network packets such that every execution unit is entirely independent of source and library chagnes to others.
    
- 
