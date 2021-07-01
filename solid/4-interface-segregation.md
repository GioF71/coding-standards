# Interface segregation principle

## Principle (from [Wikipedia](https://www.wikipedia.org/))
In the field of software engineering, the interface-segregation principle (ISP) states that no client should be forced to depend on methods it does not use. ISP splits interfaces that are very large into smaller and more specific ones so that clients will only have to know about the methods that are of interest to them. Such shrunken interfaces are also called role interfaces. ISP is intended to keep a system decoupled and thus easier to refactor, change, and redeploy. ISP is one of the five SOLID principles of object-oriented design, similar to the High Cohesion Principle of GRASP.  

## Importance in object-oriented design
Within object-oriented design, interfaces provide layers of abstraction that simplify code and create a barrier preventing coupling to dependencies.  
According to many software experts who have signed the Manifesto for Software Craftsmanship, writing well-crafted and self-explanatory software is almost as important as writing working software. Using interfaces to further describe the intent of the software is often a good idea.  
A system may become so coupled at multiple levels that it is no longer possible to make a change in one place without necessitating many additional changes.[1] Using an interface or an abstract class can prevent this side effect.  

## References

The text of this page has been adapted from [this](https://en.wikipedia.org/wiki/Interface_segregation_principle) article on  [Wikipedia](https://www.wikipedia.org/).  
The principle has been introduced by [Robert C. Martin](https://en.wikipedia.org/wiki/Robert_C._Martin).  
