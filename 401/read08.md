# Read: 08 - OO Design

## SOLID: The First 5 Principles of Object Oriented Design

the first five object-oriented design and what SOLID stands for:

- S - Single-responsiblity Principle
- O - Open-closed Principle
- L - Liskov Substitution Principle
- I - Interface Segregation Principle
- D - Dependency Inversion Principle

#### S - Single responsibility principle
the Single Responsibility Principle states that every module or class should have responsibility.
#### O — Open/closed principle
In programming, the open/closed principle states that software entities (classes, modules, functions, etc.) should be open for extensions, but closed for modification.
#### L — Liskov substitution principle
In programming, the Liskov substitution principle states that if S is a subtype of T, then objects of type T may be replaced (or substituted) with objects of type S.
#### I — Interface segregation principle
In programming, the interface segregation principle states that no client should be forced to depend on methods it does not use.
#### D - Dependency inversion principle
In programming, the dependency inversion principle is a way to decouple software modules.


## The SOLID Principles in Real Life:

#### s is for single responsibility principle
the single responsibility principle (srp) asserts that a class or module should do one thing only.

A toaster has toggles to change the length of time the bread stays in the toaster; it has buttons to eject the toast early. Each of those pieces all directly affects the primary operation of the toaster, to toast your bread! Toasting your bread is the only thing the toaster does, it doesn’t make your coffee too!

### o is for open/closed principle
the open/closed principle states that code entities should be open for extension, but closed for modification.
A package holiday includes certain things: a hotel, travel arrangements, etc. The travel company cannot remove those expected items. Open to extension means that the travel company can add additional items. For example they could throw in a complimentary car for your holiday at no cost to you.

### l is for liskov substitution principle
the liskov substitution principle (lsp) is the one here that is most unique to object-oriented programming. 
Liskov Substitution states that you should be able to substitute an object for any descendant object without your implementation knowing any different. A descendant object is an object that inherits from another object and extends it. E.g. List inherits from and extends IEnumerable.
A particular taxi app offers these options: standard (base type), large (fit’s larger groups) (descendant), and executive (descendant), etc. The company must send a car that fit’s larger groups if you choose the large option. The only requirement of the standard option is for a car that can get you from A to B. Any car, whether from the standard, large or executive options fulfills that requirement as the other options inherit and extend from the standard option.

### i is for interface segregation principle
the interface segregation principle (isp) says that you should favor many, smaller, client-specific interfaces over one larger, more monolithic interface. 
Interface segregation
Car manufacturers offer many different options on their cars, and most aggregate these options into common “packs,” e.g. A winter pack with heated steering wheel and front windscreen. You’re not forced to choose from packs that have options you’re not going to use, as you can choose individual options.

### d is for dependency inversion
the dependency inversion principle (dip) encourages you to write code that depends upon abstractions rather than upon concrete details. 
Dependency inversion is an object not creating other objects that it relies upon; Instead, they’re passed in by an outside source, e.g. relying on an email service interface and the email service object being passed in by your dependency injection container. 
