- **object** - An object is an entity with state and behaviour, such as a chair, a bike, a marker, a pen, a table, a car, and so on. It could be either physical or logical (tangible or intangible). The financial system is an example of an intangible object.
-  **State:** The data (value) of an object is represented by its state.
- **Behaviour:** The functionality of an object, such as deposit, withdrawal, and so on, is represented by the term behaviour.
- **Identity:** A unique ID is often used to represent an object’s identification. The value of the ID is hidden from the outside user. The JVM uses it internally to uniquely identify each object.
- **class** - A class is a collection of objects with similar attributes. It’s a blueprint or template from which objects are made. It’s a logical thing. It can’t be physical. In Java, a class definition can have the following elements:
- **Modifiers:** A class can be private or public, or it can also have a default access level
- **class keyword:** To construct a class, we use the class keyword.
- **class name:** The name of the class should usually start with a capital letter.
- **Superclass (optional):** If the class has any superclass, we use the extends keyword and we mention the name of the superclass after the class name.
- **Interface (optional):** If the class implements an interface, we use the implements keyword followed by the name of the interface after the class name.

* IN-DEPTH :
	- **Constructors:** A constructor in Java is a block of code that is comparable to a method. When a new instance of the class is created, the constructor is invoked. It is only when the constructor is invoked that memory for the object is allocated.
	- **this** : The this keyword is used to refer to the current instance variable of the class. It can be also used to call the current method of the class. This() is also called the constructor of the current class (super() is used to call the superclass constructor)
	- **final** : When a variable is declared using the final keyword, the value of the variable cannot be changed, making it a constant. A final class is one that has been declared with the final keyword. It is not possible to extend a final class. A method is called a final method when it is declared with the final keyword. It is not possible to override a final method.![[Screenshot 2024-05-28 at 6.42.20 PM.png]]
	- **Static** : When a variable is marked as static, a single copy of the variable is made at the class level and shared among all objects. The static method is defined as a method that is declared using the static keyword. The main() method is the most common example of a static method. Any static member of a class can be accessed before any objects of that class are generated, and without requiring a reference to any object.
	- **super** : In Java, the super keyword is a reference variable that refers to parent class instances.