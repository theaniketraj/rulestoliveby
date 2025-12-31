# The Fallacies of Distributed Computing

> "The network is reliable. Latency is zero. Bandwidth is infinite. The network is secure. Topology doesn't change. There is one administrator. Transport cost is zero. The network is homogeneous."

**The Insight:**  
L. Peter Deutsch listed these 8 false assumptions that programmers make when moving from single-machine code to distributed systems. Believing any of these leads to systems that fail in production.

**In Practice:**  
Always set timeouts (network is not reliable). Retry with backoff (latency is not zero). Encrypt internal traffic (network is not secure). Don't hardcode IP addresses (topology changes).
