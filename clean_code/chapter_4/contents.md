# Comments
## Comments Do not Make Up for Bad Code
- Clear and expressive code with few comments is far superior to cluttered and complex code with lots of comments.
- Rather than spend your time writing the comments that explain the mess you've made, spend it cleaning that mess.
- 
## Explain Yourself in Code

## Good Comments
- Legal Comments
- Informative Comments
  - It is sometimes useful to provide basic information with a comment.
- Explanation of Intent
  - It is sometimes useful to provide the intent behind a decision.
- Clarification
  - ```
    assertTrue(a.compareTo(a) == 0); // a == a
    assertTrue(a.compareTo(b) != 0); // a != b
    ```
- Warning of Consequences
  - It is sometimes useful to warn other programmers about certain consequences.
- TODO Comments
  - Explain why the function has a degenerate implementation and what the function's future should be.
  - Jobs that the programmer thinks should be done, but for some reason can't do at the moment.
  - Whatever else a TODO might be, it is not an excuse to leave bad code in the system!!!
- Amplification
  - Amplify the importance of something that many otherwise seem inconsequential.
- Javadocs in Public APIs

## Bad Comments
- Most comments fall into this category.
- Mumbling
  - If you decide to write a comment, then spend the time necessary to make sure it is the best comment you can write.
- Redundant Comments
- Misleading Comments
- Mandated Comments
  - silly -> javadoc or every variable must have a comment
- Journal Comments
  - Nowadays, we don't need to create log entries.
- Noise Comments
  - Restate the obvious and provide no new information -> Nothing but noise.
- Scary Noise
- Don't use a Comment When You Can Use a Function or Variable
  - ```
    // Bad case
    // does the module from the global list <mod> depend on the
    // subsystem we are part of?
    if (smodule.getDependSubsystems().contains(subSysMod.getSubSystem()))

    // Better
    ArrayList moduleDependees = smodule.getDependSubsystems(); String ourSubSystem = subSysMod.getSubSystem();
    if (moduleDependees.contains(ourSubSystem))
    ```
