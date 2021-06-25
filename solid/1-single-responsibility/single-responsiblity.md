# Single-responsibility principle

## Principle (from [Wikipedia](https://www.wikipedia.org/))
The single-responsibility principle (SRP) is a computer-programming principle that states that every module, class or function in a computer program should have responsibility over a single part of that program's functionality, and it should encapsulate that part. All of that module, class or function's services should be narrowly aligned with that responsibility.[1]

Robert C. Martin, the originator of the term, expresses the principle as, "A class should have only one reason to change,"[1] although, because of confusion around the word "reason" he also stated "This principle is about people.". In some of his talks, he also argues that the principle is, in particular, about roles or actors. For example, while they might be the same person, the role of an accountant is different from a database administrator. Hence, each module should be responsible for each role.

## Example (from [Wikipedia](https://www.wikipedia.org/))
Martin defines a responsibility as a reason to change, and concludes that a class or module should have one, and only one, reason to be changed (e.g. rewritten).

As an example, consider a module that compiles and prints a report. Imagine such a module can be changed for two reasons. First, the content of the report could change. Second, the format of the report could change. These two things change for different causes. The single-responsibility principle says that these two aspects of the problem are really two separate responsibilities, and should, therefore, be in separate classes or modules. It would be a bad design to couple two things that change for different reasons at different times.

The reason it is important to keep a class focused on a single concern is that it makes the class more robust. Continuing with the foregoing example, if there is a change to the report compilation process, there is a greater danger that the printing code will break if it is part of the same class. 

## References

The text of this page has been adapted from [this](https://en.wikipedia.org/wiki/Single-responsibility_principle) article on  [Wikipedia](https://www.wikipedia.org/).  
The term "single-responsability principle" has been introducted by [Robert C. Martin](https://en.wikipedia.org/wiki/Robert_C._Martin).  
Further readings and examples: [Envato envatotuts+](https://code.tutsplus.com/tutorials/solid-part-1-the-single-responsibility-principle--net-36074)
