# Moore's Law

> "The number of transistors on a microchip doubles about every two years, though the cost of computers is halved."

**The Insight:**  
Gordon Moore's 1965 observation drove the entire digital revolution. It became a self-fulfilling prophecy for the semiconductor industry. It means computing power grows exponentially while cost drops exponentially.

**In Practice:**  
In software, this meant "wait and hardware will solve your performance problem." Today, Moore's Law is slowing (or dead) for single-thread performance. We can no longer rely on free speedups; we must rely on parallelism (see Amdahl's Law) and efficiency (see The Bitter Lesson).
