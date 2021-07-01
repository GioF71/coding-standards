# Liskov substitution principle

## Principle (from [Wikipedia](https://www.wikipedia.org/))
Liskov's notion of a behavioural subtype defines a notion of substitutability for objects; that is, if S is a subtype of T, then objects of type T in a program may be replaced with objects of type S without altering any of the desirable properties of that program (e.g. correctness).

Behavioural subtyping is a stronger notion than typical subtyping of functions defined in type theory, which relies only on the contravariance of parameter types and covariance of the return type. Behavioural subtyping is undecidable in general: if q is the property "method for x always terminates", then it is impossible for a program (e.g. a compiler) to verify that it holds true for some subtype S of T, even if q does hold for T. Nonetheless, the principle is useful in reasoning about the design of class hierarchies.

Liskov substitution principle imposes some standard requirements on signatures that have been adopted in newer object-oriented programming languages (usually at the level of classes rather than types; see nominal vs. structural subtyping for the distinction):

* Contravariance of method parameter types in the subtype.
* Covariance of method return types in the subtype.
* New exceptions cannot be thrown by the methods in the subtype, except if they are subtypes of exceptions thrown by the methods of the supertype.

In addition to the signature requirements, the subtype must meet a number of behavioural conditions. These are detailed in a terminology resembling that of design by contract methodology, leading to some restrictions on how contracts can interact with inheritance:

* Preconditions cannot be strengthened in the subtype.
* Postconditions cannot be weakened in the subtype.
* Invariants must be preserved in the subtype.
* History constraint (the "history rule"). Objects are regarded as being modifiable only through their methods (encapsulation). Because subtypes may introduce methods that are not present in the supertype, the introduction of these methods may allow state changes in the subtype that are not permissible in the supertype. The history constraint prohibits this. It was the novel element introduced by Liskov and Wing. A violation of this constraint can be exemplified by defining a mutable point as a subtype of an immutable point. This is a violation of the history constraint, because in the history of the immutable point, the state is always the same after creation, so it cannot include the history of a mutable point in general. Fields added to the subtype may however be safely modified because they are not observable through the supertype methods. Thus, one can define a circle with immutable center and mutable radius as a subtype of an immutable point without violating the history constraint.

## References

The text of this page has been adapted from [this](https://en.wikipedia.org/wiki/Liskov_substitution_principle) article on  [Wikipedia](https://www.wikipedia.org/).  
The principle has been introduced by [Barbara Liskov](https://en.wikipedia.org/wiki/Barbara_Liskov).  
