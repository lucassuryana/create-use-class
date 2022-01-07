## Creating and Using a Class

This work is adapted from "Python Crash Course: A Hands-On, Project-Based Introduction to Programming" by Eric Matthes.

Object-oriented programming (OOP) is one of the best approaches to code software. In OOP, we will write classes that will represent real-world things and situations. Then we will write objects based on these classes. When writing classes, we will define the behavior that objects can have/do.

The process of making an object from classes is called instantiation, and we will work with the instances of a class. In this part, we will learn how to write classes and create instances from those classes.

### Creating the Dog Class

Each instance created from the Dog class wil store a name and an age. We will give each dog the ability to sit() and roll_over(). Copy and paste the code below to dog.py file.
```markdown
class Dog: #1
    """A simple attempt to model a dog.""" #2
    
    def __init__(self, name, age): #3
      """Initialize name and age attributes."""
      self.name = name #4
      self.age = age
    
    def sit(self): #5
        """Simulate a dog sitting in response to a command."""
        print(f"{self.name} is now sitting.")
        
    def roll_over(self):
        """Simulate rolling over in response to a command."""
        print(f"{self.name} rolled over!")
  
```

If you notice, there is a hashtag (#) with a number inside the code. Below is the explanation:
#1 -> Create a class called Dog. By convention, the class is written in capitalized named and it does not need parentheses because we write it from the scratch.
#2
#3
#4
#5
