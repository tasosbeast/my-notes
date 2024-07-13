# arithmetic operators in order from highest precedence (18) to lowest precedence (1):

# Arithmetic Operators by Precedence

| Precedence | Operator                                             | Name                            | Description                                 | Example                     | Result                         |
| ---------- | ---------------------------------------------------- | ------------------------------- | ------------------------------------------- | --------------------------- | ------------------------------ | --- | --- | --- | ------------ |
| 18         | `()`                                                 | Parentheses                     | Defines the order of operations             | `(5 + 3) * 2`               | `16`                           |
| 17         | `++` `--`                                            | Increment/Decrement             | Increases or decreases value by one         | `a = 5; a++`                | `a = 6`                        |
| 16         | `**`                                                 | Exponentiation                  | Raises to the power of                      | `5 ** 2`                    | `25`                           |
| 15         | `*` `/` `%`                                          | Multiplication/Division/Modulus | Multiplies, divides or finds remainder      | `5 * 3` `6 / 3` `5 % 2`     | `15` `2` `1`                   |
| 14         | `+` `-`                                              | Addition/Subtraction            | Adds or subtracts                           | `5 + 3` `5 - 3`             | `8` `2`                        |
| 13         | `<<` `>>` `>>>`                                      | Bitwise Shift                   | Shifts bits left, right, or zero-fill right | `a << b` `a >> b` `a >>> b` | -                              |
| 12         | `<` `<=` `>` `>=`                                    | Relational                      | Compares values                             | `a < b`                     | `true/false`                   |
| 11         | `==` `!=`                                            | Equality                        | Checks if values are equal or not           | `a == b`                    | `true/false`                   |
| 10         | `&`                                                  | Bitwise AND                     | AND operation on bits                       | `a & b`                     | -                              |
| 9          | `^`                                                  | Bitwise XOR                     | XOR operation on bits                       | `a ^ b`                     | -                              |
| 8          | `                                                    | `                               | Bitwise OR                                  | OR operation on bits        | `a                             | b`  | -   |
| 7          | `&&`                                                 | Logical AND                     | AND operation on boolean values             | `a && b`                    | `true/false`                   |
| 6          | `                                                    |                                 | `                                           | Logical OR                  | OR operation on boolean values | `a  |     | b`  | `true/false` |
| 5          | `?:`                                                 | Conditional                     | Ternary conditional                         | `a ? b : c`                 | -                              |
| 4          | `=` `+=` `-=` `*=` `/=` `%=` `<<=` `>>=` `&=` `^=` ` | =`                              | Assignment                                  | Assigns values              | `a = b` `a += b`               | -   |
| 3          | `yield`                                              | Yield                           | Pauses and resumes a generator function     | `yield value`               | -                              |
| 2          | `,`                                                  | Comma                           | Separates expressions                       | `a, b`                      | -                              |
