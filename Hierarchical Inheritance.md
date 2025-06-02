# Exp.No:5(e)	HIERARCHICAL INHERITANCE
- **Name:** S.Y.Anuranjana
- **Registration Number:** 212222050006

### AIM
To write a Python program to Get the employee  and doctor details & display it using Hierarchical inheritance.create a parent (base) class name Details and two child (derived) classes named Employee and Doctor
### ALGORITHM

Step 1:	  Begin the program.

Step 2:	 Create a class Details with an __init__ method to initialize three attributes: id, name, and gender.

Step a:	Define a method display_details() to print the values of id, name, and gender.

Step 3:	 Create a class Employee that inherits from the Details class.

Step a:	Add two additional attributes: company and department.

Step b:	Override the display_details() method to print the employee-specific attributes (company and department) along with the inherited details.

Step 4:	 Create a class Doctor that also inherits from the Details class.

Step a:	Add two additional attributes: hospital and department.

Step b:	Override the display_details() method to print the doctor-specific attributes (hospital and department) along with the inherited details.

Step 5:	 Accept input for employee and doctor details.

Step 6:	Create objects of Employee and Doctor using the input.

Step 7:	Call the display_details() method for both objects to print the details.Step 8:	

### PROGRAM
# Parent class Details
class Details:
    def __init__(self, id, name, gender):
        self.id = id
        self.name = name
        self.gender = gender

    def display_details(self):
        print(f"Id:  {self.id}")
        print(f"Name:  {self.name}")
        print(f"Gender:  {self.gender}")

# Child class Employee
class Employee(Details):
    def __init__(self, id, name, gender, company, department):
        # Call parent class constructor
        super().__init__(id, name, gender)
        self.company = company
        self.department = department

    def display_details(self):
        print("Employee Object")
        super().display_details()
        print(f"Company:  {self.company}")
        print(f"Department:  {self.department}")

# Child class Doctor
class Doctor(Details):
    def __init__(self, id, name, gender, hospital, department):
        # Call parent class constructor
        super().__init__(id, name, gender)
        self.hospital = hospital
        self.department = department

    def display_details(self):
        print("Doctor Object")
        super().display_details()
        print(f"Hospital:  {self.hospital}")
        print(f"Department:  {self.department}")

# Main function to get input and display details
def main():
    # Create Employee object and display details
    employee_id = int(input())
    employee_name = input()
    employee_gender = input()
    employee_company = input()
    employee_department = input()

    employee = Employee(employee_id, employee_name, employee_gender, employee_company, employee_department)
    employee.display_details()
    print("")
    # Create Doctor object and display details
    doctor_id = int(input())
    doctor_name = input()
    doctor_gender = input()
    doctor_hospital = input()
    doctor_department = input()

    doctor = Doctor(doctor_id, doctor_name, doctor_gender, doctor_hospital, doctor_department)
    doctor.display_details()

# Run the main function
main()

### OUTPUT
 ![image](https://github.com/user-attachments/assets/49f2eb5f-b9a6-4e0e-8b36-cae4cbe497e1)

### RESULT
Thus the python program for Hierarchical Inheritance to get the employee details was implemented and executed successfully.
