# The DRY Principle

> "Don't Repeat Yourself."

**The Insight:**  
Every piece of knowledge must have a single, unambiguous, authoritative representation within a system. If you copy-paste logic, you now have two places to maintain it. When one changes and the other doesn't, you have a bug.

**In Practice:**  
Abstract common logic into functions. Use variables for constants. However, adhere to "AHA" (Avoid Hasty Abstractions). Duplication is far cheaper than the wrong abstraction. Apply DRY when business logic is duplicated, not just when code looks similar.
