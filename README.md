# How to write JS like a pro :rocket:

### always use triple equals
No exceptions
```
if (a === b) {
    // ...
}
```


### null check
Always check with triple equals

```
if (x === null) {
    // ...
}
```
    
### undefined check
Always check with triple equals and use `typeof`.

```
if (typeof x === 'undefined') {
    // ...
}
```

*Why?*
`undefined` is not a reserved word and it can be used as an identifier.
```
undefined = 123;
const x = undefined;
if (x === undefined) {
    console.log('x is undefined');
} else {
    console.log('x is not undefined');
}

// output: x is not undefined
```

### use `let` and `const`
Assign each variable as `const` if possible. If not use `let`.

### use desctructing assignment
```
const a = {
    x: 1,
    y: 2,
    z: 3
};
const { x, y, z } = a;
console.log(x, y, z); // 1 2 3
```

### `async` and `await`
Prefer using `async` and `await` over `promise.then(...)`.
