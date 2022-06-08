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

Why?
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