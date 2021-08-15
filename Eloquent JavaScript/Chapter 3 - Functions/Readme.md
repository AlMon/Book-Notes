# Functions

Functions are the bread and butter of JavaScript because wrapping a piece of a program inside a value has many uses. It allows us to give structure to larger programs, to reduce repetition and to associate names with subprograms.

Defining new vocabulary is the most obvious application of functions, it is indispensable for programming.

Functions have a set of parameters and a body, the body contains the statements that are going to be executed when the function is called. Parameters are optional, albeit often used.

Functions produce either a value through said value being returned or they result in a side effect. Functions with a blank return statement or functions without a return statement at all return undefined. Therefore all functions have a return statement innately.

Scope is all about visibility and usability. Some variables have scope inside all parts of a program, they are call “global” variables. Variables used within a function only have scope inside that function and they are known as “local” variables.

In that same vein, all variables are local to the block that they are declared in.

Before ES6, variables had global scope regardless of where they were declared in. That used to be a regular nightmare for a lot of programmers who had to deal with the unforeseen side effects of that kind of implementation.

Multiple degrees of locality can be produced by creating scopes within scopes.

JavaScript is extremely broad-minded about the number of arguments you pass to a function. If you pass too many, the extra ones are ignored. If you pass too few, the missing parameters get assigned the value undefined.

A good mental model is to think of function values as containing both the code in their body and the environment in which they are created. When called, the function body sees the environment in which it was created, not the environment in which it is called.

Performance in an interesting balancing act. Almost any program can be made faster by convoluting it, yet we have to keep in mind the fact that our eyes are never going to be the only ones that are going to look at the code that’s in front of us.

Worrying about efficiency can be a distraction. It’s yet another factor that complicates program design, and when you’re doing something that’s already difficult, that extra thing to worry about can be paralyzing.

In other words, premature optimization is never the answer. Always start by writing something that’s correct and easy to understand.

More code means more space for mistakes to hide in and more material for people to read and try to understand.

A useful principle is to not add cleverness unless you are absolutely sure you’re going to need it.

Functions that create values are easier to combine in new ways than functions that directly perform side effects.

A pure function is a specific kind of value-producing function that not only has no side effects but also doesn’t rely on side effects from other code—for example, it doesn’t read global bindings whose value might change. A pure function has the pleasant property that, when called with the same arguments, it always produces the same value (and doesn’t do anything else).
