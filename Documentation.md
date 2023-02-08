# Introduction
Mythos is a general-purpose, statically-typed, compiled programming language. It features functions, types, returns, blocks, and a grammar that makes it easy for developers to write and understand code.

# Functions
In Mythos, a function can be defined using the `fn` keyword. The function definition consists of the function name, arguments, and the code block that implements the function.

The syntax for a function definition is:
```php
fn functionName(arg1/dataType1, arg2/dataType2, ...) returnDataType {
    // function implementation
    return expression;
}
```
For example, the following is a function that adds two integers and returns the result:
```java
fn add(a/int, b/int) int {
    return a + b;
}
```
Additionally, Mythos also supports one-statement functions, which are concise and ideal for simple operations. A one-statement function consists of the function definition and a single expression, which is automatically returned by the function.

The syntax for a one-statement function is:

`fn functionName(arg1/dataType1, arg2/dataType2, ...) returnDataType => statement;`

For example, the following is a one-statement function that adds two integers and returns the result:

```java
fn add(a/int, b/int) int => return a + b;
```

Here's an additional example that will print a string with a new line:

```c
fn print(text/string) => printf("%s\n", text);
```

# Types

In Mythos, there are several built-in data types: `int`, `string`, `null`, and `bool`.

The `int` type represents integers, and can be positive or negative.

The `string` type represents sequences of characters.

The `null` type represents the absence of a value.

The `bool` type represents true or false values.

Custom types are planned.

# Returns

A function can return a value using the return keyword followed by an expression. The expression must match the return data type specified in the function definition.

For example, the following function returns an integer:
```java
fn add(a/int, b/int) int {
    return a + b;
}
```

# Blocks
A block in Mythos is a sequence of statements surrounded by curly braces {}. The statements in a block are executed in order, and can contain return statements to end the function early.

#External Functions
The `extern` keyword is used in Mythos to declare an external function. An external function is a function that is defined in another language or library and is used in Mythos via its declaration.

The syntax for declaring an external function is:
`extern fn functionName returnDataType;`

For example, the following brings in `printf` which allows us to print into the console.
```java
extern fn printf int;
```

# Error Handler
Pretty much non-existant as of right now.
