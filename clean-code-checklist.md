# Code Review Checklist (from Clean Code: A Handbook of Agile Software Craftsmanship by Robert Martin)

### Naming things

- Name reveals intent - does the name of the variable, function, or class tell you why it exists, what it does, and how it's used?
- Avoid mental mapping - generally write a name that matches what it's supposed to do, and avoid single digit variable names.
- Avoid verbs in class names - because...
- Method naming - methods should have verb or verb phrase names

### Functions

- What does the function do? - a function should either (1) do something or (2) answer a question -- not do both (1) and (2)
- Function size - rule of thumb might be that more than twenty lines is too long.
- Do one thing ... what else to say?
- Indent levels - more than two indent levels, and it might be too big.
- Stick to one level of abstraction - try not to mix high and low level things in the same function.
- Follow the step down rule - organize the class or file to start with the highest level of abstraction and then descend into lower levels of abstraction.
- Fewest possible number of function arguments - zero arguments is best, one argument is good, two arguments and you're getting too complex, three or more arguments... ugh. Why? Lots of reasons, but increased complexity to comprehend the function and complexity in unit testing might be of the strongest.
- Avoid side effects - if your function is doing more than the name suggests (e.g., updating instance variables that nobody expected), then you might consider refactoring.
- Avoid output arguments - e.g., return values should generally be the result of an operation, not a transformation -- better would be to have a method that changes the state of its own object.

### Credits

Shout out to the LA Software Craftsmanship meetup for graciously granting us permission to use this checklist. If you're out on the westside, please consider joining their [meetup](http://www.meetup.com/LA-Software-Craftsmanship/).
