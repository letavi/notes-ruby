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
