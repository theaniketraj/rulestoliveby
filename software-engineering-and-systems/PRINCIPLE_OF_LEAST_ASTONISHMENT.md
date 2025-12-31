# The Principle of Least Astonishment (POLA)

> "A component of a system should behave in a way that users expect it to behave. The behavior should not astonish or surprise the user."

**The Insight:**  
If a user presses `Ctrl+S`, they expect to save. If it closes the window, they will be astonished (and angry). Good design is predictable. It leverages the user's existing mental models.

**In Practice:**  
Follow conventions. If you are building a CLI, use standard flags (`-h` for help). If you are building an API, use standard HTTP verbs (`GET` for read, `POST` for create). Don't try to be "unique" with fundamental interactions. Boredom is better than surprise.
