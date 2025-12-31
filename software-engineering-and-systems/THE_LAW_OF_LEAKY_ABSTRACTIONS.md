# The Law of Leaky Abstractions

> "All non-trivial abstractions, to some degree, are leaky."

**The Insight:**  
We build abstractions (like TCP/IP, ORMs, or High-Level Languages) to simplify complex systems by hiding implementation details. However, Joel Spolsky argues that you can never completely hide the underlying reality. When things go wrong—network latency, database index misses, memory leaks—the abstraction "leaks," forcing you to understand the layer below to fix it.

**In Practice:**  
Don't be afraid of the black box. While you should use abstractions to move fast, you must invest time in learning how they work under the hood. If you use an ORM, learn SQL. If you use React, learn the DOM. True mastery requires understanding the layer _one level deeper_ than where you work.
