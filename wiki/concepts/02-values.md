# 02: Values & Basic Data Types

## Related Code
- `examples/02-values.go`

## Question Asked
**"What are the basic value types in Go and how do they work with operations?"**

## Answer & Explanation

Go has several built-in value types that form the foundation of the language. Your `02-values.go` example demonstrates three fundamental categories:

### String Values and Operations
```go
fmt.Println("go" + "lang")  // String concatenation with +
```

- Go uses the `+` operator for string concatenation
- String literals are enclosed in double quotes `""`
- Strings in Go are immutable - concatenation creates new strings
- Result: `"golang"`

### Numeric Values and Arithmetic
```go
fmt.Println("1+1 =", 1+1)         // Integer arithmetic
fmt.Println("7.0/3.0 =", 7.0/3.0) // Floating-point arithmetic
```

**Integer Operations:**
- `1+1` performs integer addition
- Go supports standard arithmetic operators: `+`, `-`, `*`, `/`, `%`
- Result: `2`

**Floating-Point Operations:**
- `7.0/3.0` performs floating-point division
- The `.0` makes these floating-point literals, not integers
- Floating-point division gives decimal results
- Result: `2.3333333333333335`

### Boolean Values and Logic
```go
fmt.Println(true && false)  // Logical AND
fmt.Println(true || false)  // Logical OR
fmt.Println(!true)          // Logical NOT
```

**Logical Operations:**
- `&&` (AND): returns `true` only if both operands are `true` → `false`
- `||` (OR): returns `true` if either operand is `true` → `true`
- `!` (NOT): inverts the boolean value → `false`

## Key Points

- **Type System**: Go is statically typed - each value has a specific type
- **No Automatic Conversion**: `1` (int) and `1.0` (float) are different types
- **Operator Overloading**: The `+` operator works for both numbers and strings
- **Boolean Logic**: Go uses `&&`, `||`, and `!` for logical operations
- **Immutability**: String operations create new values rather than modifying existing ones

## Type Behavior Details

### Why `7.0/3.0` and not `7/3`?
- `7/3` would be **integer division** → result: `2` (truncated)
- `7.0/3.0` is **floating-point division** → result: `2.333...`
- Go doesn't automatically convert between integer and floating-point types

### String Concatenation Performance
- Each `+` operation creates a new string
- For multiple concatenations, consider using `strings.Builder` or `fmt.Sprintf`

## Try It Yourself

1. **Experiment with mixed operations:**
   ```go
   fmt.Println("Result: " + string(42))  // This will cause an error!
   ```
   Why does this fail? How would you fix it?

2. **Test integer vs float division:**
   ```go
   fmt.Println("Integer:", 7/3)
   fmt.Println("Float:", 7.0/3.0)
   ```

3. **Boolean combinations:**
   ```go
   a, b := true, false
   fmt.Println("NAND:", !(a && b))
   fmt.Println("XOR:", (a || b) && !(a && b))
   ```

## Questions to Explore Next

- How do you convert between different number types in Go?
- What other arithmetic operators does Go support?
- How do you work with strings that contain special characters?
- What happens when you try to add different types together?
- How does Go handle integer overflow?

## Additional Notes

**Performance Insight**: String concatenation with `+` is fine for a few strings, but for building longer strings in loops, Go's `strings.Builder` is more efficient.

**Type Safety**: Go's strict typing prevents many runtime errors by catching type mismatches at compile time.