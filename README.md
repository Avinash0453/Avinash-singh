class Employee {
 private String name;
 private double salary;
    public Employee() {
        this.name = "Unknown"; // Default name
        this.salary = 0.0;     // Default salary
    }
    public Employee(String name) {
        this.name = name;
        this.salary = 30000.0; // Default salary
    }
    public void displayEmployeeDetails() {
        System.out.println("Employee Name: " + this.name);
        System.out.println("Employee Salary: " + this.salary);
    }
}
public class EmployeeTest {
    public static void main(String[] args) {
        Employee emp1 = new Employee();
        System.out.println("Details of Employee 1:");
        emp1.displayEmployeeDetails();
        System.out.println();
        Employee emp2 = new Employee("Alice");
        System.out.println("Details of Employee 2:");
        emp2.displayEmployeeDetails();
    }
}
