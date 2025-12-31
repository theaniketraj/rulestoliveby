# The Law of Demeter

> "Each unit should have only limited knowledge about other units: only units 'closely' related to the current unit."

**The Insight:**  
Also known as the "Principle of Least Knowledge." In code, this often means "don't talk to strangers." An object should only call methods on its internal components, not components of those components (Avoid `user.getWallet().getBank().getBalance()`).

**In Practice:**  
Reduce coupling. If you change a lower-level object, you shouldn't have to rewrite code three layers up. Use wrapper methods or dependency injection to keep meaningful "distance" between unrelated parts of your system.
