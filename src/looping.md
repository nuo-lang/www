# Looping

## Infinite

```
loop {
    stdout.write_line("Keeps going.");
}
```

## Generators

Arrays are a type of finite generator.

```
const friends = ["Bob", "Alice", "Sally"];

loop friend of friends {
    stdout.write_line(`I have a friend named {friend}.`);
}
```

Any range between two i64 or u64 values is also a finite generator. Ranges are denoted using the `..` operator ("range operator").

```
loop 0 .. 5 {
    stdout.write_line("Hi.");
}

loop num of 0 .. 5 {
    stdout.write_line(`num: {num}`);
}
```

## Conditions

You can also specify a condition while looping. The condition will be evaluated before each iteration, and the loop will stop when the condition evaluates to `false`.

```
const start = time.now();
const end = start.add_minutes(5);

var iterations = 0;

loop start < end {
    iterations++;
};

stdout.println(iterations);
```

## Expression

```
const friends = ["Bob", "Alice", "Sally"];

const firstAName = loop friend of friends {
    if friend.startsWith("A") {
        return friend;
    }
}

stdout.println(`My first friend whose name starts with an A is {firstAName}`);
```
