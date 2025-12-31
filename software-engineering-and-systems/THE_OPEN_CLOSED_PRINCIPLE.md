# The Open/Closed Principle (OCP)

> "Software entities (classes, modules, functions, etc.) should be open for extension, but closed for modification."

**The Insight:**  
You should be able to change what a module _does_ without changing its _source code_. This sounds impossible, but it's achieved via polymorphism and inheritance.

**In Practice:**  
Instead of a giant `if/else` block checking `if (type == 'pdf') ... else if (type == 'html')`, define an interface `ReportGenerator` with a `generate()` method. Pass in a `PdfGenerator` or `HtmlGenerator`. To add a new format, you just add a new class; you don't touch the existing (working) code.
