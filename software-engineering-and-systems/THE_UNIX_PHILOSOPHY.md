# The Unix Philosophy

> "Write programs that do one thing and do it well. Write programs to work together. Write programs to handle text streams, because that is a universal interface."

**The Insight:**  
Douglas McIlroy summarized this approach to software design. It focuses on modularity and composition. Instead of building massive, monolithic applications that try to do everything, build small, sharp tools that can be chained together (piped) to solve complex problems.

**In Practice:**  
Build functions and classes that have a single responsibility. Make your components composable. If you are building a platform, expose an API/CLI that allows users to script and combine your tools in ways you never anticipated.
