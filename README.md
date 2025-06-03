# CPP 04

## Project Overview

**CPP 04** explores subtype polymorphism, abstract classes, and interfaces in C++. I implemented a hierarchy of animal classes demonstrating polymorphic behavior through virtual functions.

This project focused on:
- Designing derived classes that inherit and extend base class attributes and behaviors
- Overriding constructors, destructors, and virtual member functions to achieve polymorphism
- Implementing dynamic memory management with deep copies for class members
- Creating abstract base classes and interfaces to enforce design constraints and enable flexible implementations
- Adding specialized member functions unique to derived classes to demonstrate extended functionality

---

### Exercise 00: Polymorphism
**Goal:** Implement a base `Animal` class and derived `Dog` and `Cat` classes, showcasing polymorphic behavior through `makeSound()`.

**Key concepts:**
- Virtual functions and dynamic dispatch (`makeSound()`)
- Protected attributes and inheritance
- Implementation of a “wrong” hierarchy (`WrongAnimal` and `WrongCat`) to demonstrate what happens without proper polymorphism

---

### Exercise 01: I don’t want to set the world on fire
**Goal:** Introduce a `Brain` class as a dynamic member of `Dog` and `Cat` for deep state management.

**Key concepts:**
- Composition: `Dog` and `Cat` own a pointer to a `Brain` object
- Dynamic memory allocation (`new` and `delete`) inside classes
- Deep copy implementation to avoid shallow copies and double deletes
- Array of polymorphic objects, proper deletion via base class pointers

---

### Exercise 02: Abstract class
**Goal:** Modify the `Animal` class to become abstract, preventing direct instantiation while maintaining polymorphic behavior.

**Key concepts:**
- Pure virtual functions (making `Animal` abstract)
- Ensuring all derived classes implement abstract methods 
- Maintaining polymorphism and behavior from previous exercises

---

### Exercise 03: Interface & recap
**Goal:** Implement an interface-like hierarchy with a magical Materia system (`AMateria`, `Character`, `MateriaSource`) showcasing pure abstract classes, cloning, inventory management, and interaction.

**Key concepts:**
- Pure abstract classes as interfaces (`AMateria`, `ICharacter`, `IMateriaSource`)
- Implementing concrete classes: `Ice`, `Cure`, `Character`, `MateriaSource`
- Prototype pattern: cloning Materias via `clone()` method
- Inventory management with fixed size and safe adding/removing
- Deep copy semantics for inventory and materials
- Method overriding with polymorphic behavior (`use()`)
- Complex interaction between objects using interfaces

