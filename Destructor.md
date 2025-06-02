# Exp.No:5(b)	Destructor
- **Name:** Naveen P
- **Registration Number:** 212222050039

### AIM
To create  a  Python Class Student with a destructor.
### ALGORITHM
Step 1:	 Begin the program.

Step 2:	 Define the student class:

Step 3:	 Inside the class student, define the __init__ method (constructor) and the __del__ method (destructor).

Step 4:	 Create an object s2 of the student class. When the object s2 is created, the __init__ method is called, and its print statements are executed.

Step 5:	 Use the del statement to delete the object s2. This triggers the __del__ method (destructor), and the respective print statements are executed.

Step 6:	  Terminate the program.

### PROGRAM
```
class student:
    def __init__(self):
        print("Inside Constructor")
        print("Object initialized")
        print("Hello, my name is Emma")
    def __del__(self):
        print("Inside destructor")
        print("Object destroyed")
s2=student()
del s2
```
### OUTPUT
 ![image](https://github.com/user-attachments/assets/bff64e83-c99e-4102-ab1d-ec15d0c3fae4)

### RESULT
Thus the python program for Class Student with a destructor, was implemented and executed successfully.
