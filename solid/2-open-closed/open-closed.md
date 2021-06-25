# Open-closed principle

## Principle (from [Wikipedia](https://www.wikipedia.org/))
In object-oriented programming, the open–closed principle states "software entities (classes, modules, functions, etc.) should be open for extension, but closed for modification";[1] that is, such an entity can allow its behaviour to be extended without modifying its source code.  
The name open–closed principle has been used in two ways. Both ways use generalizations (for instance, inheritance or delegate functions) to resolve the apparent dilemma, but the goals, techniques, and results are different.  
Open–closed principle is one of the five SOLID principles of object-oriented design.  

## Meyer's open–closed principle
 (from [Wikipedia](https://www.wikipedia.org/))

Bertrand Meyer is generally credited for having originated the term open–closed principle, which appeared in his 1988 book Object Oriented Software Construction.  

* A module will be said to be <b>open</b> if it is still available for extension.  
For example, it should be possible to add fields to the data structures it contains, or new elements to the set of functions it performs.  
  
* A module will be said to be <b>closed</b> if it is available for use by other modules.  
This assumes that the module has been given a well-defined, stable description (the interface in the sense of information hiding).  

At the time Meyer was writing, adding fields or functions to a library inevitably required changes to any programs depending on that library.Meyer's proposed solution to this dilemma relied on the notion of object-oriented inheritance (specifically implementation inheritance):  

* A class is closed, since it may be compiled, stored in a library, baselined, and used by client classes. But it is also open, since any new class may use it as parent, adding new features.  
When a descendant class is defined, there is no need to change the original or to disturb its clients.

## References

The text of this page has been adapted from [this](https://en.wikipedia.org/wiki/Open%E2%80%93closed_principle) article on  [Wikipedia](https://www.wikipedia.org/).  
The term "open-closed principle" has been introducted by [Bertrand Meyer](https://en.wikipedia.org/wiki/Bertrand_Meyer).  
