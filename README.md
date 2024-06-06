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
