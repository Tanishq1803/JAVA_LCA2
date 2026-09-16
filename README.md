```java
class Person
{
    String name;
    int age;

    void displayPerson()
    {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
    }
}

class Student extends Person
{
    int rollNo;
    String course;

    void displayStudent()
    {
        displayPerson();
        System.out.println("Roll No: " + rollNo);
        System.out.println("Course: " + course);
    }
}

class Employee extends Person
{
    int empId;
    String department;

    void displayEmployee()
    {
        displayPerson();
        System.out.println("Employee ID: " + empId);
        System.out.println("Department: " + department);
    }
}

public class Main
{
    public static void main(String[] args)
    {
        Student s = new Student();

        s.name = "Rahul";
        s.age = 18;
        s.rollNo = 101;
        s.course = "Computer Engineering";

        System.out.println("STUDENT INFORMATION");
        s.displayStudent();

        System.out.println();

        Employee e = new Employee();

        e.name = "Amit";
        e.age = 30;
        e.empId = 201;
        e.department = "IT";

        System.out.println("EMPLOYEE INFORMATION");
        e.displayEmployee();
    }
}
```
