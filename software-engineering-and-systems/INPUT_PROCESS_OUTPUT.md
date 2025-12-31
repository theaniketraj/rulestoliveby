# Input-Process-Output (IPO)

> "All systems generally have an Input, a Processing step, and an Output."

**The Insight:**  
This is the fundamental model of computation and systems theory. It cleanly separates concerns: getting data in, doing something with it, and getting results out. Errors usually happen at the boundaries (Input/Output), while complexity hides in the middle (Process).

**In Practice:**  
Structure your functions this way. Validate inputs rigorously at the gate. Keep your processing logic "pure" (side-effect free) if possible. Format outputs only at the very end. The more you mix these stages (e.g., printing to screen _during_ a calculation), the harder your code is to test and reuse.
