# The Single Responsibility Principle (SRP)

> "A class should have one, and only one, reason to change."

**The Insight:**  
Responsibility = Reason to change. If a `User` class handles both "saving to database" and "generating a PDF report," it violates SRP. If the database schema changes, `User` changes. If the PDF format changes, `User` changes. This coupling leads to fragile code.

**In Practice:**  
Split them up. `UserRepository` handles the DB. `UserReportGenerator` handles the PDF. `User` should just be data. Small, focused classes are easier to test and understand.
