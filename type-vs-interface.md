### Title :Type Alias vs Interface in TypeScript. Core Differences and When to Use Them.





#### ***Introduction:***





In Typescript type alias \& interface are two different path to make Custom Type. They can ensure Object , structure \& type safety.



but their Declaration Merging, Primitive Types, Union Types, Intersection Types \&  Type Composition are different.



Advanced Type Manipulation:



Type Alias support advance type manipulation e.g :keyof, Conditional Types \& Mapped Types,but interface cannot directly define these type expressions.



type User = {

&#x20; name: string;

&#x20; age: number;

};



type UserKeys = keyof User;

##### 

##### **When Should we Choose One Over the Other:**



**For Interface:**



* Define Obj structure.
* Contract defying for class
* For interface extending
* Declaration Merging will be required.



**For Type Alias:**



* Creating Union Type
* Define Tuple
* Creting primitive type of alias
* Creating Intersection Type,etc.





#### **Conclusion:**



overall, type Alias and Interface has Important part of typescript.Interface is more suitable for defining object structures, extensibility, and declaration merging. On the other hand, Type Alias is more flexible for defining unions, intersections, tuples, primitives, and advanced type manipulations.





