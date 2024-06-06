- **ABSTRACT CLASS**
	- An abstract class instance cannot be created.
	- The use of constructors is permitted.
	- There is no need for an abstract method in an abstract class.
	- Final methods aren't allowed in abstract classes since they can't be overridden, but abstract methods are designed to be overridden.
	- We are prohibited from creating objects for any abstract class

- **INTERFACE**
	- An interface, like a class, can include methods and variables, but the methods declared in an interface are abstract by default (only method signature, no body).
	- Interfaces define what a class must do, not how it must do it.
	- An interface is about capabilities; for example, a Player may be an interface, and any class that implements it must be able to (or must implement) movement (). As a result, it provides a set of methods that must be implemented by the class.
	- If a class implements an interface but does not offer method bodies for all of the interface's functionalities, the class must be abstracted.

- _**Reasons for introducing interfaces in Java:**_
	- It's a technique for achieving complete abstraction.
	- Because java does not provide multiple inheritances in the case of classes, multiple inheritances can be achieved by using interfaces.
	- It can also be used for loose coupling.

