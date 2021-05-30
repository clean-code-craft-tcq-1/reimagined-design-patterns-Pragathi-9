# reimagined-design-patterns

Give a summary description of Four design patterns that you choose from the following design patterns: **Adapter,  Builder, Composite, Decorator, Observer, Interpreter, State, Mediator, Memento, Prototype, Proxy**. In your summaries say:

- what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example
- how the pattern works, what the basic idea of the pattern is
- what the main advantage and what the the main disadvantage is of using this pattern
- Write a short summary for each of the four patterns, about half a page for each pattern (rather less than more). 

> Do not add diagrams, and do not try to give a complete description of the patterns as found in the books. Rather think of how you would explain the essential ideas of these patterns in a few sentences to a colleague while drinking coffee.

/**************************************************************************************************************************************************************
/

Below mentioned are four design patterns that  I feel are most efficient Software design patterns:

1. **Adapter Design pattern:**
    1. This pattern acts as a bridge between two incompatible interfaces.
    2. it involves an adapter class which establishes communication between two independent interfaces.
    
    *Example:*
    Consider current code that is designed to provide weather conditions when a city name is entered.
    Now if the user desires to input a zipcode instead of city name, the code has to respond with weather conditions too.
    Here a class convertZipcodetoCityname has to be designed that converts zip code to a city name and then the city name can be input to
    existing implementationto acquire weather conditions output.
    
    *Advantages:*
    1. helps in making the code much structured, supports open close principle.
    2. addition of new adapter class without disturbing existing code. Hence, makes it much flexible.
    
    *Disadvantages:*
    > Could increase the complexity as new classes or interfaces are added evertime.
 
 2. **Builder Design Pattern:**
    1. Builder pattern is a creational design pattern. 
    2. This pattern enables the polymorphism. 
    3. Builder pattern builds a complex object using simple objects and using a step by step approach.
    
    *Examples:*
    Let's consider a business case of fast-food restaurant where a typical meal could be a burger and a cold drink. Burger could be either a Veg Burger or
    Chicken Burger and will be packed by a wrapper. Cold drink could be either a coke or pepsi and will be packed in a bottle.
    We are going to create an Item interface representing food items such as burgers and cold drinks and concrete classes implementing the Item interface and a
    Packing interface representing packaging of food items and concrete classes implementing the Packing interface as burger would be packed in wrapper and
    cold drink would be packed as bottle.
    
    *Advantage:*
    1. It improves modularity by separating the complex object creation from required object representation
    2. Easy to modify and maintain since the construction process is isolated
    3. Improves readability and testability
    
    *Disadvantage:*
    > Increase of classes to represent different forms of the same object would make performance overhead
    
 3. **Decorator Design Pattern**
    1. Decorator patterns allow a user to add new functionality to an existing object without altering its structure. So, there is no change to the original
    class.
    2. The decorator design pattern is a structural pattern, which provides a wrapper to the existing class.
    3. Decorator design patterns create decorator classes, which wrap the original class and supply additional functionality by keeping the class methods’
    signature unchanged.
    
    *Examples:*
    Let say, I have a engine-less car, I want to add either the Petrol engine or Diesel engine to this car. Then what I need to do is, I have to introduce the
    Car Decorator. This Car Decorator will add Engine to the Car. Let's say I want to add a Petrol Engine then the Car Decorator will add the Petrol Engine to
    this car and return the car with a petrol engine. Suppose, I want to add a Diesel Engine to this car, then the Car Decorator will add a Diesel engine to
    this car and return the car with the Diesel engine.
    
    *Advantages:*
    1. high degree of flexibility
    2.  significantly improves the readability of the program code
    
    *Disadvantages:*
    1. Using the pattern increases the complexity of the software.
    2. large number of decorator objects, for which a separate systematization is recommended to avoid similar overview problems when working with subclasses.
    
4. **Observer Design Pattern:**
   1. An observer design pattern is a behavioral design pattern where objects are represented as observers that wait for an event to trigger. When the new 
      eventis triggered, the multiple observers catch these events.
   2. The event source (or object) attaches to the subject. Whenever the change is performed in the subject, it is notified by the observer. 
   3. It follows the one to many approaches between the objects so that one change in the subject will reflect in all of its dependents and be updated
     automatically.
     
    *Example:*
    If we are newspaper or magazine subscriber, we don't need to go the store to get the news. We get the newspaper at home. If there is a new update
    available, the publisher sends it directly to our mailbox right after publication.
    The publisher has the complete information regarding the subscriber. The subscriber can stop the publisher's service if it doesn't match with their
    interest.

   *Advantages:*
   1. It is quite flexible to set up the relationship at runtime between the objects.
   2. With the Open/Closed Principle's help, we can introduce the new subscriber class without making a change in the publisher's code.
   3. This method carefully describes the coupling existing between the objects and the observer.

    *Disadvantages:*
    1. The observer method has a risk to implement. If it is not implemented carefully, it will be the cause of large complexity code.
    2. The main disadvantage of the observer design pattern that subscribers are notified in random order.


    
    
    
    
