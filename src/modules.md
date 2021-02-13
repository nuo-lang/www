# Modules

Modules are specified via URLs or file paths.

```
const uuid = import("https://nuopkgsexample.com/uuid.nuo");

export type task = struct {
    id: string,
    title: string,
};

export const create(title: string): task {
    return task {
        id: uuid(),
        title,
    };
}
```
