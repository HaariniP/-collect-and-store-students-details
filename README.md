# -collect-and-store-students-details
package students details;
import java.util.Scanner;
class Student {
    private String name;
    private int rollNumber;
    private int age;
    public void create() {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter name: ");
        this.name = scanner.nextLine();
        System.out.print("Enter roll number: ");
        this.rollNumber = scanner.nextInt();
        System.out.print("Enter age: ");
        this.age = scanner.nextInt();
    }
    public void display() {
        System.out.println("Name: " + this.name);
        System.out.println("Roll number: " + this.rollNumber);
        System.out.println("Age: " + this.age);
    }
}
public class students details {
    public static void main(String[] args) {
        Student[] students = new Student[2];
        for (int i = 0; i < students.length; i++) {
            students[i] = new Student();
            students[i].create();
        }
        System.out.println("\nStudent Details:");
        for (int i = 0; i < students.length; i++) {
            System.out.println("Student " + (i + 1) + ":");
            students[i].display();
            System.out.println();
        }
    }
}

Output 
Student Details:
Student 1:
Name: John Doe
Roll number: 101
Age: 20

Student 2:
Name: Jane Smith
Roll number: 102
Age: 22

