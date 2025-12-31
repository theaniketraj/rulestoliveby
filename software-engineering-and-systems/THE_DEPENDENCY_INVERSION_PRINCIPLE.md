# The Dependency Inversion Principle (DIP)

> "High-level modules should not depend on low-level modules. Both should depend on abstractions."

**The Insight:**  
Your business logic (High Level) shouldn't care if you are using MySQL, PostgreSQL, or a flat file (Low Level). If `OrderService` specifically instantiates `MySQLDriver`, you are stuck.

**In Practice:**  
`OrderService` should depend on an interface `IDatabase`. You inject the specific implementation (`MySQLDriver`) at runtime (Dependency Injection). This inverts the control flow and decouples your architecture.
