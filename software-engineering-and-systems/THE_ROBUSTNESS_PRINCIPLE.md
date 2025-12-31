# The Robustness Principle (Postel's Law)

> "Be conservative in what you do, be liberal in what you accept from others."

**The Insight:**  
Jon Postel formulated this for TCP/IP adoption. If every node strictly rejected slightly malformed packets, the internet would never have worked. By accepting "good enough" input but producing "perfect" output, different systems can interoperate even if they are slightly buggy.

**In Practice:**  
In API design: Validate inputs flexibility (e.g., ignore unknown JSON fields instead of crashing) but strictly define your output schema. This allows you to evolve your API (adding new fields) without breaking old clients.
