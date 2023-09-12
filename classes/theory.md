# Classes in Python

### Object

- An object can be thought of as a container.
- This container can contain "data" which are sometimes called as "state" which can be accessed through "attribute"
- This container can also contain functionality which can also refer to its behavior.
- Consider an object called as "my_car": 
  - my_car:
    - states
      - brand = Ferrari
      - model = 599XX
      - year = 2010
    - behavior
      - accelerate
      - brake
      - steer
- Accessed through dot notation.
  - my_car.brand -> Ferrari
  - my_car.accelerate(10)
- Creating objects:
  - How can we create the "container"?
  - How do we define and set state?
  - How do we define and implement behavior?
  - How do we differentiate between both state and behavior?
- Many languages use a class-based approach. A "class" is like a template used to create objects. Also called as "type".
- Objects created from the class are called instances of that class or type.
- Classes are themselves objects. They have attributes(state). They have behavior.
- If a class is an object, and objects are created from classes, how are classes created?
- Python classes are created from the type "metaclass". (More on it later).
- Instances:
  - classes have behavior. They are callable. This returns an instance of the class often called objects, differentiating from class.
  - Instances are created from classes, their type is the class they were created from.
    - If `MyClass` is a "class" in Python and `my_obj` is an instance of that class:
        ```
      my_obj = MyClass()
      type(my_obj) -> MyClass
      isinstance(my_obj, MyClass) -> True
      ```
- Creating Classes
  - Use the `class` keyword.
  - ```
    class MyClass:
      pass
    ```
  - Python creates an object called `MyClass` of type `type` and automatically provides us certain attributes(state) and methods(behavior)
  - State: `MyClass.__name__` -> `MyClass`
  - Behavior: `MyClass()` -> Returns an instance of `MyClass`
 