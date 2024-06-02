Object Oriented Programming - Artefacts 

On this page are a number of artefacts that I have gather from my studies of Object Oriented Programming as part of my MSc Computer Science course. These show my development relating to coding practice, UML and computing theory that aligns with OOP.

### Artefact 1: Reflections on the Power of E-Portfolios

[E-Portfolio Development Reflection](/pdf/e_portfolio_development.pdf)

### Artefact 2: Collaborative Discussion regarding Reusability of Code in OOP

[Collaborative Discussion](/pdf/collaborative_discussion.pdf)

### Artefact 3: UML Models within the Software Development Life Cycle

[UML and SDLC](/pdf/uml_in_sdlc.pdf)

### Artefact 4: Python Code Showing Protected and Unprotected Variables

```
    class Student:
      def __init__(self, name, age, ID):
        self.name = name # this is an unprotected variable
        self.age = age # this is unprotected
        self._ID = ID # the “_” prior to “ID” highlights this as a protected variable
    
    s1 = Student("Billy", 15, 1443)
    
    print(s1.name)
    print(s1.age)
    print(s1._ID)
```

---
### Artefact 5: Polymorphism Example

```
        class SteerLeft:
            def __init__(self, direction, degrees):
                self.direction = direction 
                self.degrees = degrees
        
            def info(self):
                print(f"Turning {self.direction} for {self.degrees}.")
        
        
        
        class SteerRight:
            def __init__(self, direction, degrees):
                self.direction = direction # this has been reused from the SteerLeft class as a form of polymorphism
                self.degrees = degrees
        
            def info(self):
                print(f"Turning {self.direction} for {self.degrees}.")
            
        
        Left1 = SteerLeft("Left", 90)
        Right1 = SteerRight("Right", 90)
        
        for directional in (Left1, Right1):
            directional.info()
```


For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).
