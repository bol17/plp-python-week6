# Week 6 Assignment: Error Handling & Debugging

## Files
- `safe_tools.py`: Contains three error-handling functions (`safe_divide`, `safe_number`, and `get_field`) that prevent program crashes using `try` and `except` blocks.

## Reflection
A standard `if` check cannot catch `"abc"` on its own when attempting to convert text to an integer because Python does not know whether a string contains valid numeric characters until `int()` actively tries to parse it. Without a `try/except` block, passing non-numeric text directly to `int()` immediately triggers an unhandled `ValueError` and crashes the program.