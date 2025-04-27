# Meaningful Names
## Use Intention-Revealing Names
- Intention!!!
- Q. What if the name should be related to business?

## Avoid Disinformation
- accountList < accounts (list means something specific to programmers)
- Beware of using names which vary in small ways.
- Spelling similar concepts similarly is information.
- Q. Does the length of the variable not matter?
  - Shorter names are generally better than longer ones, so long as they are clear. Add no
more context to a name than is necessary.

## Make Meaningful Distinctions
- If name must be different, then they should also mean something different.
- Info, Data -> reflect on myself...
- Distinguish names in such a way that the reader knows what the differences offer.

## Use Pronounceable Names

## Use Searchable Names

## Avoid Encoding

## Interfaces and Implementations
- IShapeFactory, ShapeFactory < ShapeFactory, ShapeFactoryImpl(CShapeFactory)

## Avoid Mental Mapping
- Professionals uses their powers for good and write code that others can understand.

## Class Names
- Classes and objects should have noun or noun phrase names, avoid using verb.
- Avoid words like Manager, Processor, Data or Info -> Why?

## Method Names
- verb or verb phrase
- When constructors are overloaded, use static factory methods with names that describe the arguments. 
  - ```
    Complex fulcrumPoint = Complex.FromRealNumber(23.0)
    ```
## Don't Be Cute

## Pick One Word per Concept

## Don't Pun

## Use Solution Domain Names
- Remember that the people who read your code will be programmers.
- Choosing technical names for those things is usually the most appropriate course.

## Use Problem Domain Names
- When there is no “programmer-eese” for what you’re doing, use the name from the problem domain.
- Separating solution and problem domain concepts is part of the job of a good programmer and designer.

## Add Meaningful Context
- Enclose in well named classes, functions, or namespaces.

## Don't Add Gratuitous Context

## Final Words
- Renaming is also a kind of code improvement.
- It will pay off in short term and continue to pay in the long run.
