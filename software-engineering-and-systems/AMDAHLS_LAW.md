# Amdahl's Law

> "The theoretical speedup of the execution of a task is limited by the part of the task that cannot benefit from the improvement."

**The Insight:**  
You can't speed up a system infinitely just by adding more power (or processors). If 5% of your program is sequential (cannot be parallelized), the maximum theoretical speedup is 20x, no matter how many thousands of CPUs you throw at it. The slowest non-improvable part dictates the limit of the whole.

**In Practice:**  
Before you optimize, profile. Find the bottleneck. If you are optimizing a part of the code that only runs 10% of the time, even deleting it entirely will only give you a 1.1x speedup. Focus on the sequential bottlenecks that block scalability.
