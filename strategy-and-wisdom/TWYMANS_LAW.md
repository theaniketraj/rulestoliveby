# Twyman's Law

> "Any datum or figure that looks interesting or different is usually wrong."

**The Insight:**  
If a chart shows a massive spike, or a metric suddenly doubles, or a correlation looks perfect, your first instinct should not be "We are geniuses!" it should be "We broke the tracking."

**In Practice:**  
Validate "interesting" data furiously. If the data confirms your bias or looks too good to be true, check the SQL query, check the logging pipeline, and check the definition of the metric. It's almost always a bug.
