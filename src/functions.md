# Functions

Functions are like snippets of code. We provide many with Nuo, and you can find more online.

## Example

```
// this example "calls" the "stdout.write_line" function
// it passes one input - a string to show in the console

stdout.write_line("Hello, world! 👋 🌎");
```

## Inputs and Outputs

Functions can take inputs and return outputs.

```
// "string.reverse" takes one input (a string), and returns one output (another string)
// in this example, we assign the output to a constant called "result"

const result = string.reverse("racecar!");
// -> "!racecar"

stdout.write_line(result);
```

## Declaring Functions

You can declare your own functions.

```
// the "sayHi" function takes no inputs and returns no outputs

const sayHi = () => {
    stdout.write_line("Hello!");
};

// say "hi" three times

sayHi();
sayHi();
sayHi();

// the "meet" function takes one input (a string for the "name") and returns no outputs

const meet = (name: string) => {
    const message = `Hello, {name}!`; // this is called a template string. we will go over this later.
    stdout.write_line(message);
};

// meet a few people

meet("Alice");
meet("Bob");
meet("Sally");

// the "is_palindrome" function takes one input (a string) and returns one output (a boolean), which will be "true" if the input string is a palindrome

const is_palindrome = (text: string): bool => {
    return text == string.reverse(text);
};

if is_palindrome("racecar") {
    stdout.write_line("racecar is a palindrome!");
}

if is_palindrome("nope") {
    stdout.write_line("nope is a palindrome!");
}
```
