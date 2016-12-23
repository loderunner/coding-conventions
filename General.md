# General guidelines

## Indentation and scope

### 1. When to indent

* Increase indentation by one level every time there is a lingering open context, i.e. parenthesis, brace, array literal, argument list, block, scope...
* Decrease indentation by one level every time a context was closed.

Examples:

C:
```c
void say_hello()
{
    const char* hello = "Hello World!";
    printf("%s\n", hello);
}
```

Javascript:
```javascript
for (var i of numbers)
{
    console.log({
        type : "number",
        value : i
    })
}
```

### 2. Use spaces, not tabs

Spaces will make your code readable on any machine, any editor, any web page display, regardless of the tab size.

Example:

Code written with tabs, tab width = 4:
```objc
- (void)resetColor
{
    self.color = [self getDefaultColorWithAlpha:1.0
                            andVeryLongArgument:@"long"
                                              x:0
                                              y:0];
}
```

Code opened in editor with tab width = 2:
```objc
- (void)resetColor
{
  self.color = [self getDefaultColorWithAlpha:1.0
              andVeryLongArgument:@"long"
                        x:0
                        y:0];
}
```

Use spaces to keep your code structured, whatever you view it in.

### 3. Recommended indentation

Recommended indentation is 4 spaces.
