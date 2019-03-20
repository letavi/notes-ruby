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
