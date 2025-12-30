# Rules to Live By

Welcome to my personal knowledge base of mental models, laws, and principles. This repository serves as a guide to navigating complex systems, software engineering challenges, and life in general.

---

## 🧭 General Principles

### 1. Murphy's Law

> "Anything that can go wrong will go wrong."

**The Insight:**  
It’s not about pessimism; it’s about preparedness. Murphy's Law reminds us that complex systems have inherent failure points. If a outcome is possible, no matter how improbable, it eventually happens given enough time and opportunity.
**In Practice:**  
Design for failure. Build redundancy, meaningful error handling, and robust backups. Assume the database will crash, the network will flake, and the user will click the wrong button.

### 2. Occam's Razor

> "Entities should not be multiplied without necessity."

**The Insight:**  
When presented with competing hypotheses that make the same predictions, one should select the solution with the fewest assumptions. Simplicity is often the hallmark of truth.
**In Practice:**  
Avoid over-engineering. If a simple script does the job, don't build a microservice architecture. Start simple and add complexity only when absolutely necessary.

### 3. The Pareto Principle (The 80/20 Rule)

> "For many events, roughly 80% of the effects come from 20% of the causes."

**The Insight:**  
Inputs and outputs are rarely distributed evenly. A small fraction of your efforts usually yields the majority of your results.
**In Practice:**  
Focus on the vital few, not the trivial many. In software, 20% of the bugs cause 80% of the crashes. Fixing that top 20% yields the massive stability wins.

---

## 🧠 Strategy & Wisdom

### 4. Chesterton's Fence

> "Do not remove a fence until you know why it was put there in the first place."

**The Insight:**  
Reforms often fail because they ignore the wisdom inherent in the status quo. G.K. Chesterton described a scene where a reformer sees a fence blocking a road and says, "I don't see the use of this; let me clear it away." The intelligent reformer replies, "If you don't see the use of it, I certainly won't let you clear it away. Go away and think. Then, when you can come back and tell me that you do see the use of it, I may allow you to destroy it."
**In Practice:**  
Before refactoring that "ugly" legacy code, understand _why_ it was written that way. It might be handling a specific edge case you haven't discovered yet. Ignorance of function is not a valid reason for destruction.

### 5. Goodhart's Law

> "When a measure becomes a target, it ceases to be a good measure."

**The Insight:**  
Any observed statistical regularity will tend to collapse once pressure is placed upon it for control purposes. If you incentivize people based on a metric, they will optimize for that metric, often at the expense of the actual goal.
**In Practice:**  
If you measure developers by "lines of code written," you will get bloated, verbose code. If you measure by "bugs fixed," you might encourage writing buggy code just to fix it later. Measure outcomes, not proxies.

### 6. The Dunning-Kruger Effect

> "The cognitive bias where people with low ability at a task overestimate their ability."

**The Insight:**  
True competence includes the ability to recognize the limits of one's own competence. Incompetence often masks itself because the skills needed to perform a task are the same skills needed to evaluate performance on that task.
**In Practice:**  
Stay humble. When you think you know everything about a new technology after a weekend tutorial, you are likely at the "Peak of Mount Stupid." Real expertise looks like "I know enough to know how much I don't know."

---

## 💻 Software Engineering & Systems

### 7. Gall's Law

> "A complex system that works is invariably found to have evolved from a simple system that worked."

**The Insight:**  
You cannot design a complex system from scratch and expect it to work. It will fail. All successful complex systems (the Internet, the Amazon ecosystem, successful operating systems) started as simple, working kernels and evolved.
**In Practice:**  
Start with a Minimum Viable Product (MVP). Get a simple "Hello World" version working end-to-end before adding bells and whistles. Don't try to build the "ultimate platform" on day one.

### 8. Conway's Law

> "Organizations which design systems are constrained to produce designs that are copies of the communication structures of these organizations."

**The Insight:**  
The architecture of a software system reflects the social boundaries of the team that built it. If you have four teams working on a compiler, you’ll get a 4-pass compiler.
**In Practice:**  
If you want a specific architecture (e.g., microservices), you must align your organizational structure to support it (the "Inverse Conway Maneuver"). Don't fight the org chart with code; fix the org chart first.

### 9. Hyrum's Law

> "With a sufficient number of users of an API, it does not matter what you promise in the contract: all observable behaviors of your system will be depended on by somebody."

**The Insight:**  
Implicit interfaces are as real as explicit ones. If your API returns a list that happens to be sorted, users will write code that _depends_ on that sorting, even if you never promised it.
**In Practice:**  
Be terrifyingly careful when changing "implementation details." There is no such thing as a strictly internal change in a widely used system. Someone, somewhere, is relying on that bug you are about to fix.

### 10. The Broken Windows Theory

> "Visible signs of crime, anti-social behavior, and civil disorder create an urban environment that encourages further crime and disorder, including serious crimes."

**The Insight:**  
In software, "broken windows" are bad designs, wrong decisions, or poor code. If left unrepaired, they signal that "no one cares," encouraging developers to write more poor code.
**In Practice:**  
Fix bad code as soon as you see it. Do not let "temporary" hacks become permanent residents. Maintain a high standard of code hygiene to encourage everyone else to do the same.

### 11. Brooks' Law

> "Adding manpower to a late software project makes it later."

**The Insight:**  
Software development is not a factory line. New people take time to ramp up (taking time away from existing team members for training) and communication overhead increases quadratically with team size ($n(n-1)/2$).
**In Practice:**  
Resist the urge to throw bodies at a deadline. It almost always generates negative productivity in the short term.
