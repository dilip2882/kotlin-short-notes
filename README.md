# kotlin-short-notes

## 1. Variables, Expressions, and Types

1. **Variables**:
   - A container for a single piece of data.
   - Must be declared before use.
   - Use `val` for read-only (immutable) variables and `var` for mutable variables.
   - Prefer `val` over `var` when possible.

2. **Declaring Variables**:
   - Start with `val` or `var`.
   - Specify variable name, data type, and initial value (optional).
   - Example: `val count: Int = 2`.

3. **Type Inference**:
   - Omit data type if initial value is provided (compiler infers type).
   - Example: `val message = "Hello, World!"`.

4. **Common Data Types**:
   - `Int`: Integer numbers.
   - `String`: Text.
   - `Boolean`: `true` or `false`.
   - `Double`: Decimal numbers with double precision.
   - `Float`: Decimal numbers with single precision.

5. **Updating Variables**:
   - Use `=` to assign a new value to a variable.
   - Only mutable variables (declared with `var`) can be updated.
   - Use increment (`++`) or decrement (`--`) operators for integer variables.

6. **String Concatenation**:
   - Use `+` to concatenate strings.
   - You can also concatenate other data types to strings.
    
7. **Expressions and Statements**:
    - Expressions can be evaluated to a value.
    - Statements do not evaluate to a value.
    - You can try assigning a chunk of code to a variable to see if it’s a statement or an expression.


## 2. Functions

1. **Function Basics**:
   - Functions are defined using the `fun` keyword.
   - They allow you to encapsulate reusable pieces of code.
   - Functions can be called from other parts of your program.

2. **Return Values**:
   - Functions can return a value using the `return` keyword.
   - Specify the return type after the function name (e.g., `fun myFunction(): Int`).
   - Use the returned value by storing it in a variable.

3. **Parameters**:
   - Functions can take parameters (inputs) to customize their behavior.
   - Parameters are declared within parentheses after the function name.
   - Example: `fun greet(name: String) { ... }`

4. **Arguments**:
   - When calling a function, provide arguments (values) for its parameters.
   - Arguments can be passed in any order using named arguments.
   - Example: `greet(name = "Alice")`

5. **Default Arguments**:
   - You can set default values for function parameters.
   - If an argument is omitted, the default value is used.
   - Example: `fun greet(name: String = "Guest") { ... }`

## 3. Conditionals

In Kotlin, branching can be achieved with `if/else` or `when` conditionals. Here are the main points:

1. **`if/else` Conditionals:**
   - The body of an `if` branch in an `if/else` conditional is executed only when the boolean expression inside the `if` branch condition returns a true value.
   - Subsequent `else if` branches in an `if/else` conditional get executed only when previous `if` or `else if` branches return false values.
   - The final `else` branch in an `if/else` conditional only gets executed when all previous `if` or `else if` branches return false values.

2. **`when` Conditionals:**
   - It's recommended to use the `when` conditional to replace an `if/else` conditional when there are more than two branches.
   - You can write more complex conditions in `when` conditionals using:
     - Comma (`,`) to match multiple cases.
     - Ranges (e.g., `1..10`) to match a range of values.
     - The `is` keyword to check type compatibility.

3. **Conditionals as Statements or Expressions:**
   - Both `if/else` and `when` conditionals can work as either statements or expressions.
   - When used as expressions, they return a value based on the condition met.
   
    Example:
    ```kotlin
    val rank = 2
    val rankLabel = when (rank) {
        1 -> "Winner"
        2 -> "First Runner Up"
        3 -> "Second Runner Up"
        else -> "Participant"
    }
    println(rankLabel)
    ```