## 8.1 Function types

To know how to declare a function that takes another function as an argument, we need to know how to declare the type of the corresponding argument.

### Declaring a function type

Let's start with examples:

Example 1: Using Kotlin's compiler to infer the types

```kotlin
val sum = { x: Int, y: Int -> x + y }
val action = { println(42) }
```

Example 2: Explicitly declaring the type

```kotlin
 val sum: (Int, Int) -> Int = { x,y -> x + y }
 val action: () -> Unit = { print(42) }
```

To declare a function type, you put the cuntion parameter types in parentheses followed by an arrow and the return type of the function. For example

```kotlin
(Int, String) -> Unit

// Int and String: Parameter type
// Unit: Return type
```
