# if / else / else if

```
if true {
    stdout.write_line("This will show up.");
}
```


```
if false {
    stdout.write_line("This won't show up.");
} else {
    stdout.write_line("This won't show up.");
}
```

```
if false {
    stdout.write_line("This won't show up.");
} else if true {
    stdout.write_line("This will show up.");
}
```

```
if false {
    stdout.write_line("This won't show up.");
} else if false {
    stdout.write_line("This won't show up.");
}
else {
    stdout.write_line("This won't show up.");
}
```

```
const message = if false {
    "Mesage 1";
} else if true {
    "Mesage 2";
} else {
    "Message 3";
}

stdout.write_line(message);

// -> "Message 2"
```
