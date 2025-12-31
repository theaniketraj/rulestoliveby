# The Interface Segregation Principle (ISP)

> "Clients should not be forced to depend upon interfaces that they do not use."

**The Insight:**  
Don't create "God Interfaces" that have 50 methods. If I only need to `print()`, I shouldn't have to implement `scan()`, `fax()`, and `staple()` just because I implemented `IMachine`.

**In Practice:**  
Break large interfaces into smaller, more specific ones. `IPrinter`, `IScanner`. A photocopier class can implement both. A simple printer class implements only `IPrinter`.
