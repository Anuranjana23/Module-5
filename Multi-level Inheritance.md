# Exp.No:5(d)	Multi-level Inheritance
- **Name:** S.Y.Anuranjana
- **Registration Number:** 212222050039

### AIM
To write a Python program to Get the name, age and id of a person and display using Multilevel inheritance.
### ALGORITHM

Step 1:	  Begin the program.


Step 2:	 Define the Person class.

Step 3:	 Inside the Person class, define the __init__ method (constructor), with  two parameters: name and age.

Step 4:	 Inside the __init__ method, assign name to self.name., assign age to self.age.

Step 5:	 Define the PersonDetails class that inherits from the Person class.

Step 6:	 Inside the PersonDetails class, define the __init__ method (constructor). with three parameters: name, age, and person_id. 

Step 7:	 Inside the __init__ method, call the __init__ method of the Person class using super() to initialize name and age, assign person_id to self.person_id.

Step 8:	 Define the DisplayDetails class that inherits from the PersonDetails class.

Step 9:	 Inside the DisplayDetails class, define the __init__ method (constructor),with three parameters: name, age, and person_id.

Step 10:	Inside the __init__ method, call the __init__ method of the PersonDetails class using super() to initialize name, age, and person_id.

Step 11:	Inside the DisplayDetails class, define the show_details method.

Step 12:	Inside the show_details method, return a formatted string with self.name, self.age, and self.person_id.

Step 13:	Prompt the user to enter name (string),age (integer),person_id (integer).

Step 14:	Create an instance person of the DisplayDetails class, passing name, age, and person_id to the constructor.

Step 15:	Call the show_details method on the person object and print the result.

Step 16:	Terminate the program.

### PROGRAM
```
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

class PersonDetails(Person):
    def __init__(self, name, age, person_id):
        super().__init__(name, age)  # Call the parent class constructor
        self.person_id = person_id

class DisplayDetails(PersonDetails):
    def __init__(self, name, age, person_id):
        super().__init__(name, age, person_id)

    def show_details(self):
        return f"{self.name} {self.age} {self.person_id}"

name = input()
age = int(input())
person_id = int(input())

person = DisplayDetails(name, age, person_id)

print(person.show_details())
```
### OUTPUT
![image](https://github.com/user-attachments/assets/e87e458f-8ee8-4d8d-b2f7-a8f80354f44c)

 
### RESULT
Thus the python program to Get the name, age and id of a person and display using Multilevel inheritance. , was implemented and executed successfully.
