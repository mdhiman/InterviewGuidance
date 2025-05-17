# How to Debug Best Practices

Debugging is a critical skill for any engineer. Here are some best practices to systematically and efficiently debug issues:

1. **Use a Debugger**  
   Step through your code using a debugger to inspect variables, call stacks, and program flow. This helps you understand exactly where things go wrong.

2. **Use Git Bisect**  
   If a bug was introduced recently, use `git bisect` to quickly identify the commit that caused the issue. This binary search approach saves time compared to manual inspection.

3. **Explain the Problem (Rubber Duck Debugging)**  
   Try to explain the bug and your code logic to someone else (or even a rubber duck). Articulating the problem often helps you see it from a new perspective and spot mistakes.

4. **Check Logs**  
   Review application, system, and error logs for clues. Logs can provide stack traces, error messages, and context about what happened before the bug occurred.

5. **Systematically Isolate and Fix the Bug**  
   Change one thing at a time and observe the effect. Isolate the problem area by disabling or modifying code sections, and use assertions or print statements if needed.

6. **Reproduce the Bug Consistently**  
   Ensure you can reliably reproduce the bug. This is essential for verifying your fix and for writing regression tests to prevent future occurrences.

---