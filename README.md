Employee Payroll Management System

 Project Description

The Employee Payroll Management System is a simple C programming project used to calculate the salary details of employees.

This program uses structures, pointers, functions, and if-else conditions to calculate:

- Gross Salary
- Performance Bonus
- Net Salary
- Employee Payslip

The program accepts details for two employees and displays their salary information.

---
 Technologies Used

- Programming Language: C
- Concepts Used:
  - Structure
  - Pointer
  - Functions
  - If-Else
  - Arithmetic Operations
  - "scanf()" and "printf()"

---

 Salary Calculation

Gross Salary

Gross Salary = Basic Salary + Allowance + Overtime

Bonus

If Performance >= 80
    Bonus = 1000
Else
    Bonus = 0

Net Salary

Net Salary = Gross Salary + Bonus - Deduction

---

 Input Details

For each employee, the program accepts:

1. Employee ID
2. Performance score (0–100)
3. Basic Salary
4. Allowance
5. Overtime
6. Deduction

---

 Output

The program displays:

- Employee ID
- Gross Salary
- Bonus
- Net Salary

---

 Sample Input

Enter details for Employee 1
Enter Employee ID: 101
Enter Performance (0-100): 85
Enter Basic Salary: 20000
Enter Allowance: 3000
Enter Overtime: 2000
Enter Deduction: 1000

Enter details for Employee 2
Enter Employee ID: 102
Enter Performance (0-100): 70
Enter Basic Salary: 18000
Enter Allowance: 2500
Enter Overtime: 1500
Enter Deduction: 500

 Sample Output

ID = 101
Gross Salary = 25000.00
Bonus = 1000.00
Net Salary = 25000.00

ID = 102
Gross Salary = 22000.00
Bonus = 0.00
Net Salary = 21500.00

---

 Concepts Demonstrated

1. Structure

The "Employee" structure stores all employee-related information in a single variable.

struct Employee {
    int id, performance;
    float basic, allowance, overtime, deduction;
    float gross, bonus, net;
};

2. Pointer

Pointers are used to pass the employee structure to functions.

salary(&e1);
salary(&e2);

The "->" operator is used to access structure members through a pointer.

3. Functions

Two functions are used:

- "salary()" – Calculates gross salary, bonus, and net salary.
- "payslip()" – Displays the employee salary details.

4. Conditional Statement

An "if-else" condition is used to calculate the performance bonus.

if (e->performance >= 80)
    e->bonus = 1000;
else
    e->bonus = 0;

---

 How to Run

Step 1: Save the Program

Save the C program as:

employee_payroll.c

Step 2: Compile

Using GCC:

gcc employee_payroll.c -o employee_payroll

Step 3: Run

./employee_payroll

On Windows:

employee_payroll.exe

---

 Objective

The main objective of this project is to demonstrate how C structures and functions can be used to create a simple payroll system and perform salary calculations efficiently.

---

Future Enhancements

The project can be improved by adding:

- Support for more employees
- Employee name and department
- Salary grade
- Different bonus percentages
- Monthly and yearly salary calculation
- Employee search functionality
- File handling for storing payroll records
- Menu-driven interface

---

