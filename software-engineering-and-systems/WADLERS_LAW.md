# Wadler's Law

> "In any language design, the total time spent discussing a feature in this list is proportional to two raised to the power of its position: 0. Semantics
>
> 1. Syntax
> 2. Lexical syntax
> 3. Lexical syntax of comments"

**The Insight:**  
Philip Wadler observed that bike-shedding scales with triviality. We spend an hour designing the type system (hard, important), and a week arguing about whether comments should start with `#` or `//`.

**In Practice:**  
When designing a system or DSL, define the difficult semantics first. Do not get bogged down in syntax debates early on. Syntax is just "sugar"; semantics are the "medicine."
