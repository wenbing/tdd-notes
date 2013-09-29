# Design Patterns

## Command

Represent the invocation of a computation as an object, not just as a message

## Value Object

Avoid aliasing problems by making objects whose values never change once created

## Null Object

Represent the base case of a computation by an object

## Template Method

Represent invariant sequences of computation with an abstract method intended to be specialized through inheritance

## Pluggable Object

Represent variation by invoking another object with two or more implementations

## Pluggable Selector

Avoid gratuitous subclasses by dynamically invoking different methods for different instances

## Factory Method

Create an object by calling a method instead of a constructor

## Imposter

Introduce variation by introducing a new implementation of existing protocol

## Composite

Represent the composition of the behavior of a list of objects with an object

## Collecting Parameter

Pass around a parameter to be used to aggregate the results of computation in many different objects


# Use of Design Patterns in Test-Driven Development

Pattern             || Test Writing || Refactoring
Command             |  X            |  
Value Object        |  X            |  
Null Object         |               |  X
Template Method     |               |  X
Pluggable Object    |               |  X
Pluggable Selector  |               |  X
Factory Method      |  X            |  X
Imposter            |  X            |  X
Composite           |  X            |  X
Collecting Parameter|  X            |  X


组合的意思是，子对象（也叫结点对象）和父对象（也叫树枝对象）可以被相同对待，也就是说，他们可能出自同一个接口或父类。



