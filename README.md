# Lab: Zoo Simulation 

## Objective
The goal of this lab is to understand and apply Dart concepts including inheritance, constructor inheritance, `super`, polymorphism, abstract classes, and mixins by creating a simulation of a zoo with different types of animals.

## Instructions

**1. Create an Abstract Base Class**
- Define an abstract class called `Animal` with:
  - An abstract method `makeSound()`.
  - A field `name` and a constructor to initialize it.
  - A method `describe()` that prints a description of the animal including its name and the sound it makes.
        
**2. Create Concrete Animal Classes**
- Define a class `Lion` that extends `Animal`. Implement the `makeSound()` method to describe the sound a lion makes. Override the method that returns the sound the lion makes.
- Define a class `Elephant` that also extends `Animal`. Implement the `makeSound()` method to describe the sound an elephant makes. Override the method that returns the sound the elephant makes.
- Use the `super` keyword in both classes to access and initialize the `name` field from the `Animal` class.
    
**3. Add a Mixin for Additional Behavior**
- Define a mixin called `Habitat`. In this mixin, create a method `getHabitat()` that returns a string representing the animal's habitat. This method should have a default implementation.
- Apply the `Habitat` mixin to both the `Lion` and `Elephant` classes. Override the `getHabitat()` method in each class to return the specific habitat of the animal (e.g., 'savannah' for lions and 'forest' for elephants).
    
***"Habitat" refers to the natural environment where an organism lives and thrives. This can include all the physical factors (such as soil, water, and climate) and biological factors (such as other organisms and food sources) that affect the life of the organism.***

    
**4. Create a Zoo Class**
- Define a class `Zoo` that contains a list of `Animal` objects.
- Add methods to add animals to the zoo and to print a description of all animals in the zoo.
- Use polymorphism to iterate over the list of animals and call the `describe()` method for each animal.
    
**5. Test the Implementation**
- In the main part of your program, create instances of `Lion` and `Elephant`. Add these instances to a `Zoo` object.
- Call the method to display descriptions of all animals in the zoo.


