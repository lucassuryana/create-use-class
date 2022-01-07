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

#1 -> Create a class called ```Dog```. By convention, the class is written in capitalized named and it does not need parentheses because we write it from the scratch.

#2 -> A docstring to describe what the class does.

#3 -> ```__init__()``` is a special method that Python runs automatically whenever we create a new instance from the Dog class. In this case it has three parameters: ```self, name, and age```. The self parameter must come first before the other parameters. It must be included in the definition because when Python calls this method later (to create an instance of ```Dog```), the method call will automatically pass the ```self``` argument. Every method call associated with an instance automatically passes ```self```, which is a reference to the instance itself; it gives the individual instance access to the attributes and methods in the class. When we make an instance of ```Dog```, Python will call the ```__init__()``` method from the ```Dog``` class. We'll pass ```Dog()``` a name and an age as arguments; ```self``` is passed automatically, so we don't need to pass it. Whenever we want to make an instance from the ```Dog``` class, we'll provide values for only last two parameters, ```name``` and ```age```.

#4 -> The defined variables in this method have the prefix ```self```. Any variable prefixed with ```self``` is available to every method in the class, and we'll also be able to access these variables through any instance created from the class.

#5 -> The ```Dog``` class has two other methods: ```sit()``` and ```roll_over()```. Because these methods don't need additional information to run, we just define them to have on parameters ```self```.
