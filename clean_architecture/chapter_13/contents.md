# Component Cohesion

## REP: The Reuse/Release Equivalence Principle
- The reuse unit is the release unit
- The classes and modules that are formed into a component must belong to a cohesive group. (overarching theme or purpose that those modules all share)
- The classes and modules that are grouped together into a component should be releasable together.

## CCP: The Common Closure Principle
- A component should not have multiple reasons to change.
- Gather together those things that change at the same times and for the same reasons.
- Seperate those things that chagne at different times or for different reasons.
- SPR, OCP

## CRP: The Common Reuse Principle
- Classes and modules that tend to be reused together belong in the same component. = Classes that are not tightly bound to each other should not be in the same component.
- Lots of dependencies on each other.

 ## Relation To ISP
 ## The Tension Diagram for Component Cohesion
 - ![image](https://github.com/user-attachments/assets/ee668209-9b93-4b1e-9c65-50f692c084bb)
 - Component structure of a project can vary with time and maturity.
