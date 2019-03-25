1. Class vs Module in Ruby

|              #              |               Class                 |                       Module               |
|-----------------------------|------------------------------------ |--------------------------------------------|
|        instantiation        |         Can be instantiated         |           Can *not* be instantiated        |
|            usage            |           Object creation           |     Mixin facility. Provides a namespace   |
|           superclass        |               Module                |                   Object                   |
|             methods         |Class methods and Instance methods   |     Module methods and Instance methods    |
|           inheritance       | Inherits behaviour and can be base for _inheritance_|       No _inheritance_     |
|           inclusion         |         Cannot be included          | Can be included in classes and modules by using the include command (includes all instance methods as instance methods in a class/module)|
|           extension         |Can not extend with extend command (only with inheritance)| Module can extend instance by using extend command (extends given instance with singleton methods from module)|

2. Ruby Array - Index

- take(n) : The first n elements of the array can be accessed using this method.
- drop(n) : Everything but except the first n elements of the array can be accessed using this method.

Example:
```
array = [1,2,3,4,5,6,7,8,9]
array.drop(2) => Result: 3,4,5,6,7,8,9
```

3. Ruby Array - Addition
- push => Add element at the ending of the array.
- unshift => Add element at the beginning of the array.

4. Rubby Array - Selection
- Non-Destructive Selection: `select`, `reject`, `drop_while`
- Destructive Selection: `select!`, `reject!`, `delete_if`, `keep_if`

5. Ruby Syntax
- All Ruby files will have extension `.rb` .
- Whitespace: Ignore in Ruby, just use to exaplain ambigous statement.
- Ruby indentifiers are case sensitive.
- Comment:
  + Single line: #
  + Multiple lines:
    ```
    =begin
    =end
    ```

6. Ruby Variables
- Local variable: Begin with lowercase letter or `_` character.
- Instance variable: Begin with `@` character.
- Class variable: Begin with `@@` character.
- Global variable: Begin with `$` character.
- Constant: Uppercase letter and can change value after initialize.

7. Ruby String
- Define a string in Ruby start with `''` or `""` .
- Defference between `''` and `""` .
  + `''` : Don't allow substitution and backslash notation.
  + `""` : Allow substitution and backslash notation. And can insert the value of any Ruby expression into a string using the `#{}` .

8. Ruby Operators
- `**`, example `2**3 =8` .
- `<=>` : Combined comparision operator. Returns `0` if first operand equals second, `1` if greater than, `-1` if less than.
- Difference between `==` and `eql?` operator:
  + `==` : Compare only value.
  + `eql?` : Compare  both value and type.
- `Parallel assignment` : It is also useful for swapping the values held in two variables.
Example:
```
a = 1
b = 2
c = 3
a, b = b, c
```
=> a = 2, b = 3, c = 3.

- `..` : Include.
- `...` : Exclude.

9. Ruy `case` statement
```
case expr0
when expr1, expr2
   stmt1
when expr3, expr4
   stmt2
else
   stmt3
end
```

10. Ruby Method
- Variable Number of Parameters: Ruby allows declare methods that work with a variable number of parameters, meaning this method, we can pass any parameters, without specified parameter.

Example:

```
def foo(*params)
end
```

So, we can call this method:
```
foo("banana", "orange")
foo("pig")
...
```

- Difference between `instance method` and `class method` and `module method` :
   + Instance Method: Provides functionality to one instance of a class.
   + Class Method: Provides functionality to a class itself

