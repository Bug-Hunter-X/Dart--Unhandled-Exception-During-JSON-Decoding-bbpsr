# Dart: Unhandled Exception During JSON Decoding

This example demonstrates a common error in Dart applications involving JSON decoding.  The application crashes due to an unhandled exception when it encounters an unexpected JSON structure from an API.

## Bug Description
The `fetchData` function attempts to fetch data from an API and decode it as JSON.  If the API returns an unexpected JSON format, the `jsonDecode` function throws a `FormatException`, causing the application to crash.

## Solution
The solution uses a `try-catch` block to handle the `FormatException`.  It gracefully handles the error by logging the exception and providing a fallback mechanism.
