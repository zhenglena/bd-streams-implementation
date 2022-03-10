### Implementing Streams

Expected time required: 15 min

Our office is in the process of uploading project files from some older hard drives to AWS. However, many of the
files don't follow our modern naming conventions, and need to be updated for our system. 

In the class `FileValidator`, there is a method `validateFiles()` that validates all files already. It uses a
number of methods that iterate over the source list and correct the names. To complete this assignment you must complete
the following methods by creating `Stream` versions of their iterative counterparts.  `validateFilesStream()` must have
the same results as `validateFiles()`.

- `createStream()`: creates a `Stream` from the list `sourceFileNames`
- `makeLowerCaseStream()`
- `removeDraftFilesStream()`
- `removeHiddenFilesStream()`
- `sortListStream()`
- `collectStreamResults()`: returns the `Stream` as a `List<String>`.

Note: Normally we wouldn't break up `Stream` operations like this into separate methods, but we wanted you to start by
practicing in bite-size chunks the different `Stream` operations.

Verify your work by running the tests in `FileValidatorTest`.

HINTS:
* [Does it matter if I implement the `Stream` operations with a method reference or lambda?](hints/hint-01.md)
