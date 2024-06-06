- String literal vs String Object![[Screenshot 2024-05-28 at 7.53.51 PM.png]]
- **String Pool:**
	- String pool is a Java heap storage area where string literals are stored. String Intern Pool or String Constant Pool are other names for it. It’s the same as object allocation. It is empty by default and is maintained privately by the Java String class. When we create a string, the string object takes up some memory in the heap. Creating a large number of strings may raise the cost and memory requirements, lowering performance.
	- During the initialization of string literals, the JVM takes several efforts to improve efficiency and reduce memory usage. The String class keeps a pool of strings to reduce the number of String objects created in the JVM.  
	- When we construct a string literal, the JVM looks it up in the String pool first. It returns a reference to the pooled instance if the literal is already existing in the pool. If the literal isn’t found in the pool, the String pool is filled with a new String object.

- **StringBuffer:** A StringBuffer is a peer class that provides a lot of the same functionality as a String. StringBuffer represents growable and writable character sequences, whereas string represents fixed-length, immutable character sequences

- **StringBuilder:** A mutable series of characters is represented by the StringBuilder in Java. Because Java’s String Class creates an immutable sequence of characters, the StringBuilder class provides an alternative by creating a mutable sequence of characters.