# struct

## Declare

```
type person = struct {
    name: string,
    age: u64,
};
```

## Instantiate

```
const p1 = person {
    name: "Bob",
    age: 42,
};

const p2 = person {
    name: "Alice",
    age: 35,
};

const p3 = person {
    name: "Sally",
    age: 78,
};

const print_person = (p: person) {
    stdout.write_line(`${p.name} is ${p.age} years old.`);
}

print_person(p1);
print_person(p2);
print_person(p3);
```
