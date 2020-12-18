# computation-dsl
A simple language to allow the core of programming - the manipulation of data - without all of the advanced features available to programmers.

# the idea
Allow users to write code in a manner similar to pseudo code (though even simpler) to manipulate data. There are no classes or inheritance - users can declare types that are simle structs to hold values and functions to operate on values. There is no access to the file system or network - the engine that runs this code will be responsible for providing the input data and then handle any output data.

# the implementors
Using a DSL allows freedom of chosing whatever language is considered 'best' for generating and running. Infact different languages/platforms could be used when running in 'Release' or 'Debug' mode. While implementing a debugger would be great (and interesting to do) for now any debugging would be done in an existing language. While not the optimal solution, debugging generated code would not be a huge stretch for the DSL author if the generated code is similar enough to what they wrote in DSL. In the worse case debugging could be handed off to someone more familiar to programming. In either case the debugging of the program could be handled via a simpler language like JavaScript or Python while production could run on code in Rust or WebAssembly.
