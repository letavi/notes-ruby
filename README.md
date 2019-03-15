1. Class vs Module in Ruby

|              #              |               Class                 |                       Module               |
|-----------------------------|------------------------------------ |--------------------------------------------|
|        instantiation        |         Can be instantiated         |           Can *not* be instantiated        |
|            usage            |           Object creation           |     Mixin facility. Provides a namespace   |
|           superclass        |               module                |                   object                   |
|             methods         | class methods and instance methods  |     module methods and instance methods    |
|           inheritance       | inherits behaviour and can be base for _inheritance_| No _inheritance_|
|inclusion| cannot be included| can be included in classes and modules by using the include command (includes all instance methods as instance methods in a class/module)|
|extension|can not extend with extend command (only with inheritance)| module can extend instance by using extend command (extends given instance with singleton methods from module)|
