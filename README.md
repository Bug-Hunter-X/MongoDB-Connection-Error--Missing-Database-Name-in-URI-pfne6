# MongoDB Connection Error: Missing Database Name

This repository demonstrates a common error when connecting to MongoDB: omitting the database name in the connection URI.

The `bug.js` file shows the erroneous code, resulting in a connection attempt that might appear to succeed but fails to select a database.  The `bugSolution.js` file provides the corrected version.

## How to Reproduce

1.  Ensure you have MongoDB installed and running.
2.  Clone this repository.
3.  Run `node bug.js`  (observe the behavior)
4.  Run `node bugSolution.js` (observe the correct behavior)

## Solution

Always specify the database name within the MongoDB connection URI.  The URI should have the format: `mongodb://<username>:<password>@<host>:<port>/<databaseName>`