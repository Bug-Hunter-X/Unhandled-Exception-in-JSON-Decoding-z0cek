# Unhandled Exception in JSON Decoding (Dart)

This repository demonstrates a common error in Dart applications: failing to handle potential exceptions during JSON decoding. The `bug.dart` file showcases the flawed code, while `bugSolution.dart` provides a corrected version.

**Problem:**
The original code attempts to decode a JSON response without error handling. If the response is not valid JSON, a `FormatException` is thrown, leading to app crashes.

**Solution:**
The solution involves wrapping the `jsonDecode` call in a `try-catch` block. This allows the application to gracefully handle `FormatException` or other exceptions that may occur during the process, preventing unexpected crashes. 