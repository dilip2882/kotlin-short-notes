# kotlin-short-notes

##1. Variables, Expressions, and Types

### Variables

- Using `var` for variables that can be reassigned.
  ```kotlin
  var count = 10
  count = 20 // Valid: Reassigning the value of 'count'
  ```
  
- Using `val` for variables that are read-only.
    ```kotlin
    val pi = 3.14
    pi = 3.14159 // Invalid: 'val' cannot be reassigned
    ```

### Expressions and Statements

- Expressions can be evaluated to a value.
- Statements do not evaluate to a value.
- You can try assigning a chunk of code to a variable to see if it’s a statement or an expression.

### Basic Types

- Number types like `Double` and `Int`.
- The `Boolean` type for true and false values.
- The `String` type for text values.
