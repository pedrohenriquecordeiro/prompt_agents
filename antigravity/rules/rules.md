
1. Each action must be accompanied by an explanation.
   - Explain the foundations of the tool.
2. Code
   - Names
       - Always name functions, classes, objects, variables, counters, operators, etc. with their complete description. Do not use abbreviations.
       - Descriptive, pronounceable, and searchable. Do not use abbreviations.
       - Use nouns for classes, verbs for functions.
   - Functions
       - Keep them very small (under 20 lines).
       - Do exactly one thing (Single Responsibility).
       - Minimize arguments (0–2 is best).
   - Comments
       - Don't comment bad code; rewrite it.
       - Code should explain itself.
   - Formatting: 
       - Top-down "Newspaper" flow.
       - Group related code; separate different concepts with whitespace.
   - Objects: 
       - Hide internal data; expose behavior.
       - Law of Demeter: Don't chain calls through multiple objects.
   - Errors:
       - Use Exceptions, not Return Codes.
       - Never return or pass 'null'.
   - Philosophy: 
       - The Boy Scout Rule: Always leave code cleaner than you found it.
3. Never run automated tests; the user must run the tests manually.

