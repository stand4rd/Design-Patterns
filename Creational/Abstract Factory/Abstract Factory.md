# Abstract Factory

## Intent
Create an interface for creating families of related OR dependent objects without providing concrete classes. 
AKA: **Kit**

## Applicability
Use an Abstract Factory pattern when:
- A system needs to be independent of how its products are created, composed, and represented.
- A system needs to be configured with one of multiple families of products
- A family of related product objects needs to be designed to be used together
- You want to provide a class library of products, and you want to reveal just thier interfaces, not thier implementations

## Participants
- **AbstractFactory**
	- Declares an interface (abstract) for operations that create abstract product objects
- **Concrete Factory**
	- Implements the operations to create "concrete" product objects
- **AbstractProduct**
	- Declares an interface for a type of product objec
- **Client**
	- Uses only interfaces declared by AbstractFactory and AbstractProduct classes

## Consequences
- It isolates concrete classes
- It makes exchanging product families easy
- It promotes consistency among products
- Supporting new kinds of products is difficult

