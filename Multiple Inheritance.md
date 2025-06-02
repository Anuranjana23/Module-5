# Exp.No:5(c)	Multiple Inheritance
- **Name:** Naveen P
- **Registration Number:** 212222050039

### AIM
To Write a Python program to get the name, attendance and Id of a student and check they are eligible for Next Module using multiple inheritance, attendance >80 eligible student else Not Eligible student
### ALGORITHM
Step 1:	 Begin the program.

Step 2:	Define the Student class.

Step 3:	Inside the Student class, define the __init__ method (constructor). The __init__ method accepts two parameters: name and student_id. 

Step 4:	Inside the __init__ method: Assign the value of name to self.name, student_id to self.student_id.

Step 5:	Define the get_student_info method inside the Student class: Return a string formatted with self.name and self.student_id.

Step 6:	Define the Attendance class, which inherits from the Student class.

Step 7:	Inside the Attendance class, define the __init__ method (constructor).

Step 8:	The __init__ method accepts three parameters: name, student_id, and attendance.

Step 9:	Inside the __init__ method: Call the parent class constructor (super().__init__(name, student_id)) to initialize name and student_id. Assign the value of attendance to 
          self.attendance.

Step 10:	Define the check_eligibility method inside the Attendance class:

Step 11:	If self.attendance is greater than 80, return a formatted string indicating the student is eligible for the module exam. Otherwise, return a formatted string indicating the 
          student is not eligible for the module exam.

Step 12:	Prompt the user to enter the name (as a string), student_id (as an integer), attendance (as an integer).

Step 13:	Create an instance student of the Attendance class, passing the entered name, student_id, and attendance to the constructor.

Step 14:	Call the check_eligibility method on the student object and print the result.
### PROGRAM
```
class Student:
    def __init__(self, name, student_id):
        self.name = name
        self.student_id = student_id
    def get_student_info(self):
        return f"Name: {self.name}, ID: {self.student_id}"
class Attendance(Student):
    def __init__(self, name, student_id, attendance):
        super().__init__(name, student_id)  
        self.attendance = attendance
    def check_eligibility(self):
        if self.attendance > 80:
            return f"{self.name}\n{self.student_id}\nEligible for Module Exam"
        else:
            return f"{self.name}\n{self.student_id}\nNot Eligible for Module Exam"
name = input()
student_id = int(input())
attendance = int(input())
student = Attendance(name, student_id, attendance)
print(student.check_eligibility())
```
### OUTPUT
![image](https://github.com/user-attachments/assets/f4959ede-568d-4162-ab31-373c5d060226)
 
### RESULT
Thus the python program to get the name, attendance and Id of a student and check they are eligible for Next Module using multiple inheritance,was implemented and executed successfully.
