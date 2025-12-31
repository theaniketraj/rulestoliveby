# The Premature Optimization Effect

> "Premature optimization is the root of all evil."

**The Insight:**  
Donald Knuth's famous warning is often misunderstood. It doesn't mean "write slow code." It means don't sacrifice readability and maintainability for small performance gains _before you know where the bottleneck is_. Optimizing 97% of your code is a waste of time because the slowdown is likely in the other 3%.

**In Practice:**  
Make it work, make it right, make it fast. In that order. Use a profiler (not your intuition) to find the slow parts. Only optimize the critical path.
