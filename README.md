## Creating and Using a Class

This work is adapted from "Python Crash Course: A Hands-On, Project-Based Introduction to Programming" by Eric Matthes.

Object-oriented programming (OOP) is one of the best approaches to code software. In OOP, we will write classes that will represent real-world things and situations. Then we will write objects based on these classes. When writing classes, we will define the behavior that objects can have/do.

The process of making an object from classes is called instantiation, and we will work with the instances of a class. In this part, we will learn how to write classes and create instances from those classes.

### Creating the Dog Class

Each instance created from the Dog class wil store a name and an age. We will give each dog the ability to sit() and roll_over(). Copy and paste the code below to dog.py file.
```markdown
class Dog:
    """A simple attempt to model a dog."""
    
    def __init__(self, name, age):
      """Initialize name and age attributes."""
      self.name = name
      self.age = age
    
    def sit(self):
        """Simulate a dog sitting in response to a command."""
        print(f"{self.name} is now sitting.")
        
    def roll_over(self):
        """Simulate rolling over in response to a command."""
        print(f"{self.name} rolled over!")
  
```
