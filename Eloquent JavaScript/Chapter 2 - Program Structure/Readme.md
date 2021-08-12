# Program Structure

A fragment of code that produces a value is known as an _expression_. Statements that are literal are expressions, be it in open scope or between parenthesis.

Much like any language, sentences can have their own subsentences to convey meaning and to describe complex computations. Expressions are to sentence fragments what JavaScript statements are to full sentences. And a program is a list of statements.

Statements amount to something only if the affect the world of the program.

The way that a program keeps internal state or, in other words, they way that it remembers things is to bind those memories to variables. Depending on the kind of variables that they are, the variables can bind new values after initial assignment.

Bindings —variables, that is— can be thought of as tentacles rather than boxes. They do not contain values per se, but rather they grasp them.

A single _let_ statement can grasp different bindings separated by commas. For example:

> let one = 1, two = 2;
> 
> console.log(one + two);
> 
> // → 3

Binding names can be any word except for strictly the same as the reserved keywords. Digits can be part of binding names—“catch22” is a valid name, for example—but the name must not start with a digit. A binding name may include dollar signs ($) or underscores (\_) but no other punctuation or special characters.

A collection of bindings and the values that they grasp is called the _environment_. A program always has an environment that contains something, even if the program itself is empty. Functions, keywords and more are part of that omnipresent environment.

A function is a piece of program wrapped in a value. Most functions are useful because of the side effects that they produce, but they can also produce values and that alone makes them useful. For example date functions or Math functions.

Functions that produce values are said to _return_ said values.

Programs are executed from top to bottom, like a story. Then again, not all programs are straight roads. This is where _conditionals_ come in handy. If/else statements are examples of conditional statements that execute the code block, which is to say the part that’s after parenthesis, depending on if the conditions between parenthesis are met.

Conditionals enable us to give our programs nuance and alternative paths within the roads we envision.

![image](https://user-images.githubusercontent.com/4275841/129141413-636559b0-6e18-4612-8299-239f954960d0.png)

The idea of programs is to make something _less_ work, not more work. Therefore loops are handy in cases we need a piece of reputable logic. Loops enable scale but they are also a kind of disruption of the regular control flow of a program.

![image](https://user-images.githubusercontent.com/4275841/129141450-7fcd63ad-927e-45b4-aea0-d9417445114a.png)

This being the case, there are two ways to break a loop. One is to finish it, i.e. to meet its final required value and the other one is to use the _break_ keyword. Loops that do not have a way to exit become infinite loops.
