# Values, Types & Operators

Everything that has to do with the computer’s world is data. We can read, modify and/or create new data, but there is nothing else going on. Thus, data is fundamentally alike.

Bits are 1s and 0s that live inside the compute, they take many forms and can be expressed in many different ways.

JavaScript uses a fixed number of bits, 64 of them to be precise. That is enough to represent about 18 quintillion (an 18 with 18 zeros after it) numbers with it.

Digital numbers, especially decimals, are only approximations, not precise values.

Wrapping numbers in parenthesis ensures that the usual arithmetic rhythm is not respected and performs that operation first before going to the next one.

We also have the _Infinity_ values represented in JavaScript, although they are not really reliable or yield meaningful results when using them.

Strings are used to represent text. Using the backslash serves as an announcement of the following character having special meaning. Escaping the character.

Strings are also sequences of numbers. Template literals also come very handy when using strings.

Boolean values are handy for situations when “yes” and “no” are sufficient.

The only value in JavaScript not equal to itself is NaN.

JavaScript has the quirk of trying to accept almost any programs that you give it, even the ones that do odd things. It uses _type coercion_ to try and guess what the value that you’re trying to use is supposed to be, convert it and use it.
