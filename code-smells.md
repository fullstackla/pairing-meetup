A "code smell" is a superficial indicator that suggests a deeper problem in your code. Learning to spot smells will be invaluable to you in improving the quality of your software.

It would serve you well to adopt best practices. However, do consider your particular context when refactoring; a prescribed solution that is generally accepted as good may not always be what you want (and similarly, one should also be careful not to blindly fall prey to dogma). Still, it is best to keep your code clear, concise, and tightly-focused. Below are more general tips to get you started.

----

### General

Keep your code as **DRY** as possible [(Do not Repeat Yourself)](http://www.artima.com/intv/dry.html).

> "DRY says that every piece of system knowledge should have one authoritative, unambiguous representation. Every piece of knowledge in the development of something should have a single representation. A system's knowledge is far broader than just its code. It refers to database schemas, test plans, the build system, even documentation." - Dave Thomas

**[Single Responsibility Principle:](https://en.wikipedia.org/wiki/Single_responsibility_principle)** classes should only be responsible for one part of your software's functionality. See also: [Separation of Concerns](https://en.wikipedia.org/wiki/Separation_of_concerns).

**Naming**: when naming classes, methods, variables, etc., use clear and descriptive names so as to keep ambiguity to a minimum. Also try to maintain a consistent naming convention.

**Unused code**: be diligent about removing dead/crufty code.

**Code length**: keep methods at around 12 lines, preferably less. Break long methods down into smaller and more focused methods; the same goes for classes. Remember: keep your code DRY and adhere to the Single Responsibility Principle.

----

### Other Tips

Write your code to solve the problem at hand and no more; do not try to solve a "problem" that hasn't even materialized yet, even if you're completely convinced of its imminence.

----

### Tools

[Reek: a code smell detector for Ruby](https://github.com/troessner/reek)
[Rubocop: linter for Ruby](https://github.com/bbatsov/rubocop)

----

### Further Reading

[Jeff Atwood - Code Smells](http://blog.codinghorror.com/code-smells/)
[Martin Fowler - CodeSmell](http://martinfowler.com/bliki/CodeSmell.html)
[JavaScript](http://rmurphey.com/js-minty-fresh/presentation/)
