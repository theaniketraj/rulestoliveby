# Hyrum's Law (The Law of Implicit Interfaces)

Hyrum's Law states that with a sufficient number of users of an API, it does not matter what you promise in the contract: all observable behaviors of your system will be depended on by somebody.

**The Insight:**  
Implicit interfaces are as real as explicit ones. If your API returns a list that happens to be sorted, users will write code that _depends_ on that sorting, even if you never promised it.

**In Practice:**  
Be terrifyingly careful when changing "implementation details." There is no such thing as a strictly internal change in a widely used system. Someone, somewhere, is relying on that bug you are about to fix.
