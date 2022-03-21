# stream-examples

# Java Stream vs Collection
A Collection is an in-memory data structure, which holds all the values that the data structure currently has. Every element in the Collection has to be computed before it can be added to the Collection. While a Stream is a conceptually a pipeline, in which elements are computed on demand.

The idea is that a user will extract only the values they require from a Stream, and these elements are only produced—invisibly to the user—as and when required. This is a form of a producer-consumer relationship.

In Java, java.util.Stream represents a stream on which one or more operations can be performed. Stream operations are either intermediate or terminal. The terminal operations return a result of a certain type and intermediate operations return the stream itself so we can chain multiple methods in a row to perform the operation in multiple steps.

Streams are created on a source, e.g. a java.util.Collection like List or Set. The Map is not supported directly, we can create stream of map keys, values or entries. Stream operations can either be executed sequentially or parallel. when performed parallelly, it is called a parallel stream.

Based on the above points, if we list down the various characteristics of Stream, they will be as follows:
-Not a data structure
-Designed for lambdas
-Do not support indexed access
-Can easily be aggregated as arrays or lists
-Lazy access supported
-Parallelizable
