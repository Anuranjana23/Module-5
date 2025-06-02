# Exp.No:5(a)	Constructors- Parameterized Constructor
- **Name:** S.Y.Anuranjana
- **Registration Number:** 212222050006
### AIM
To write a Python code to create a Class for a Person with the parameterised constructor which will take the name and userid of the person as parameters print the userid  of the person,
### ALGORITHM

Step 1:	 Begin the program.

Step 2:	 Define the person class.

Step 3:	 The class person has an __init__ method, which is the constructor. It accepts two parameters: name and userid. 

Step 4:	Inside the __init__ method: Assign the name to self.name. Assign the userid to self.userid.

Step 5:	 Print the self.userid.

Step 6:	 Prompt the user to enter the name (string) and id.

Step 7:	 Create an instance s1 of the person class by passing the entered name and userid to the constructor.

Step 8:	 Terminate the program.
### PROGRAM
```
class person:
    def __init__(self,name,userid):
        self.name=name
        self.userid=userid
        print(self.userid)
name=input()
userid=input()
s1=person(name,userid)
```
### OUTPUT
 ![image](https://github.com/user-attachments/assets/95ebab44-d7da-435c-b994-e752ebeabd44)

### RESULT
Thus the python program for parameterised constructor which will take the name and userid of the person as parameters print the userid  of the person, was implemented and executed successfully.
