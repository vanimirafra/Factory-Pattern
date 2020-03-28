# Factory-Pattern
Factory Method is a Creational Design Pattern that allows an interface or a class to create an object,
but let subclasses decide which class or object to instantiate. Using the Factory method, we have the best
ways to create an object. Here, objects are created without exposing the logic to the client and for creating
the new type of the object, the client uses the same common interface.

Advantages of using Factory method:
-------------------------------------
We can easily add the new types of products without disturbing the existing client code.
Generally, tight coupling is being avoided between the products and the creator classes and objects.

Disadvantages of using Factory method:
--------------------------------------------
To create a particluar concrete product object, client might have to sub-class the creator class.
You end up with huge number of small files i.e, cluttering of the files.

Applicability :
----------------
In a Graphics system, depending upon the user’s input it can draw different shapes like Rectangle, 
Square, Circle, etc. But for the ease of both developers as well as the client, we can use the factory 
method to create the instance depending upon the user’s input. Then we don’t have to change the client
code for adding a new shape.
In a Hotel booking site, we can book a slot for 1 room, 2 rooms, 3 rooms, etc. Here user can input 
the number of rooms he wants to book. Using the factory method, we can create a factory class AnyRooms 
which will help us to create the instance depending upon the user’s input. Again we don’t have to change the client’s
code for adding the new facility.
