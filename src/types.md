# Types

## Declarations

You must first declare a variable or constant before it can be used or reassigned.

### Declaring constants
```
const name = "Bob";
var age = 42;
var is_happy = true;
```

### Declaring variables
```
var name = "Bob";
var age = 42;
var is_happy = true;
```

### Constants vs. Variables

Variables can be reassigned new values, whereas constants cannot. If you aren't sure, use a constant.

### Type Inference

The compiler will try to guess the type of your declaration. If you want to be explicit, specify a type:

```
// guessed to be u64... if a subtraction later occurs, i64
var age = 42;

// explicitly enforced as u64
var age: u64 = 42;
```

It's currently undecided if constants are also immutable. There's a subtle difference.

## Primitive Types

Nuo's primitive types are:

| Type        | Description | Examples |
| ----------- | --- | --- |
| `bool`      | `true` or `false`. | `true`, `false` |
| `u64`       | 64-bit unsigned integer. Can only represent positive numbers. | 10, 100, 0 (min), 18446744073709551615 (max) |
| `i64`       | 64-bit integer. Can be positive or negative. | 10, 100, -40, 0, -9223372036854775807 (min), 9223372036854775807 (max) |
| `string`    | Text (represented as UTF-8)  | "hi", "Hello", "Emojis are good too 👌" |

All primitive types are immutable.
