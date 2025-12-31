# The Liskov Substitution Principle (LSP)

> "Derived classes must be substitutable for their base classes."

**The Insight:**  
If `S` is a subtype of `T`, then objects of type `T` may be replaced with objects of type `S` without altering any of the desirable properties of the program. Basically: don't break the contract. If the parent class says "I return a positive number," the child class cannot return -1.

**In Practice:**  
The classic violation is the "Square/Rectangle" problem. A Square is a Rectangle mathematically, but if you have `setWidth()` in Rectangle, using it on a Square (which changes height too) might break code that assumes width and height are independent. Inheritance is tricky; favor composition.
