## passing the string value into the Number() constructor to return a number version of the same value.

```javascript
let myNumber = "74";
myNumber = Number(myNumber) + 3;
```

## The unary plus or, in other words, the plus operator + applied to a single value, doesn’t do anything to numbers. But if the operand is not a number, the unary plus converts it into a number.

```javascript
// Converts non-numbers
alert(+true); // 1
alert(+""); // 0
```

It actually does the same thing as Number(...), but is shorter.
