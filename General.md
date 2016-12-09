# General guidelines

## Indentation

### 1. When to indent

* Increase indentation by one level every time there is a lingering open context, i.e. parenthesis, brace, array literal, argument list, block, scope...
* Decrease indentation by one level every time a context was closed.

Examples:

C:
```c
void say_hello() {
  const char* hello = "Hello World!";
  printf("%s\n", hello);
}
```

Javascript:
```javascript
for (var i of numbers) {
  console.log({
    type : "number",
    value : i
  })
}
```
