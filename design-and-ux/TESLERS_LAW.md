# Tesler's Law

> "Every application has an inherent amount of complexity that cannot be removed or hidden. Instead, it must be dealt with, either in product development or in user interaction."

**The Insight:**  
Conservation of Complexity. If you make the UI simple (one button), the backend becomes incredibly complex to interpret that button. If you make the backend simple (raw SQL), the UI becomes complex for the user. You can't destroy complexity; you can only move it.

**In Practice:**  
As a designer/engineer, your job is to _take_ the complexity so the user doesn't have to. Don't force the user to enter their city AND zip code; ask for the zip code and look up the city. You write the complex code so the user has a simple life.
