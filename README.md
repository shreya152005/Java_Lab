[PROGRAM-1: Create a class with 4 methods: addition,subtraction,multiplication,division and test all 4 methods in public static void main.](#xyz)

[PROGRAM-2: Write a program to test for, while and do-while loop for  the same problem](#abc)

[PROGRAM-3:Write a program using if else to print the grade of input marks](#x)

[PROGRAM-4:Write a program using object and classes for the following problems: a)square of stars for dynamic height and width , b)triangle of stars.](#y)

[PROGRAM-5:Write a program to add 2 distances where each distance is given in m,cm](#z)

[PROGRAM-6:Write a program to add 2 distances where each distance is given in m,cm,mm](#a)

[PROGRAM-7:Write a program to add 2 time in object oriented fashion where each time is given in hr,min](#b)

[PROGRAM-8:Write a program to add 2 time in object oriented fashion where each time is given in hr,min,sec](#c)

[Program-9:Write a Java program to create a class for a one-dimensional array with four methods: one method to take input from the user, two methods to display the array in different ways, and one method to display the array in reverse order. Test all the methods in the main method.](#d)


[PROGRAM-10:write a class with multiple methods to perform matrix operations (transpose, addition, sum of rows, sum of columns, sum of diagonal).](#m)

[PROGRAM-11: Write a program using three classes to print 1-100 ,1-100,1-100 with and without thread and analyse the output and repeat the same program using runnable interface.](#n)

[PROGRAM-12: Using the concept of multithreading the output of all three threads must be synchronised (use join method).](#o)

[PROGRAM-13:Addition of 2 numbers using swing.](#p)

[PROGRAM-14:Make one calculator in swing.](#q)

[PROGRAM-15:Matrix Addition using swing class](#r)

[PROGRAM-16:Create one jframe apply 10 buttons on that after clicking on each button a new structure is created.(Circle, oval rectangle, etc ....)](#s)

[PROGRAM-17:Just using mouse Event create a frame like paint brush with selection of colour and width .](#t)

[PROGRAM-18:Create a package of any 5 classes of your choice and import it.](#v)

[PROGRAM-19:Create one package and sub package import and test it .](#w)

[PROGRAM-20:Create one small array of size 5 apply array out of bounds exception using try catch give a proper message in catch and demonstrate the exception exactly in the same fashion demonstrate arithmetic exception .](#e)

[PROGRAM-21:To test the range of age of one student.write a program using user defined exception.](#f)

[PROGRAM-22:File Handling Programs (given in the PPT).](#g) 

[PROGRAM-23:Inheritance Programs, using interface and abstract classes.](#h)

[PROGRAM-24:Make a registration form with 10 elements and send the data into database (use jdbc connectivity)](#i)

[PROGRAM-25:Collect the code from internet for any five programs of c language. (Fact, armstrong, palindrome, Fibonacci, pattern).](#j)


# xyz 
                                              PROGRAM-1
 ```                                             
import java.util.Scanner;

class Calculator {

    // Addition
    int add(int a, int b) {
        return a + b;
    }

    // Subtraction
    int subtract(int a, int b) {
        return a - b;
    }

    // Multiplication
    int multiply(int a, int b) {
        return a * b;
    }

    // Division
    double divide(int a, int b) {
        if (b == 0) {
            System.out.println("Cannot divide by zero");
            return 0;
        }
        return (double) a / b;
    }

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        Calculator calc = new Calculator();

        // Taking input from user
        System.out.print("Enter first number: ");
        int a = sc.nextInt();

        System.out.print("Enter second number: ");
        int b = sc.nextInt();

        // Calling methods
        System.out.println("Addition: " + calc.add(a, b));
        System.out.println("Subtraction: " + calc.subtract(a, b));
        System.out.println("Multiplication: " + calc.multiply(a, b));
        System.out.println("Division: " + calc.divide(a, b));
<img width="504" height="126" alt="image" src="https://github.com/user-attachments/assets/39d09fdf-a2d9-4e4b-9b9a-0934b11a43f3" />


        sc.close();
    }
}
```

# abc

                                                 PROGRAM-2

                                                 
public class LoopTest {

    public static void main(String[] args) {

        System.out.println("Using FOR loop:");
        for(int i = 1; i <= 5; i++) {
            System.out.println(i);
        }

        System.out.println("\nUsing WHILE loop:");
        int j = 1;
        while(j <= 5) {
            System.out.println(j);
            j++;
        }

        System.out.println("\nUsing DO-WHILE loop:");
        int k = 1;
        do {
            System.out.println(k);
            k++;
        } while(k <= 5);

    }
}

Output : 
<img width="385" height="324" alt="image" src="https://github.com/user-attachments/assets/de624b63-5392-49b5-aada-e48e9e06734f" />

# x
                                                PROGRAM-3

                                                
import java.util.Scanner;

public class GradeCalculator {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter your marks: ");
        int marks = sc.nextInt();

        if (marks >= 90) {
            System.out.println("Grade: A");
        } else if (marks >= 75) {
            System.out.println("Grade: B");
        } else if (marks >= 60) {
            System.out.println("Grade: C");
        } else if (marks >= 40) {
            System.out.println("Grade: D");
        } else {
            System.out.println("Grade: Fail");
        }

        sc.close();
    }
}


Output:
<img width="311" height="33" alt="image" src="https://github.com/user-attachments/assets/587542ec-5d8d-4ee7-a460-6327221b7766" />

# y

                                              PROGRAM-4

import java.util.Scanner;

class StarPatterns {

    // Method for square of stars
    void square(int rows, int cols) {
        System.out.println("\nSquare Pattern:");
        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= cols; j++) {
                System.out.print("* ");
            }
            System.out.println();
        }
    }

    // Method for triangle of stars
    void triangle(int n) {
        System.out.println("\nTriangle Pattern:");
        for (int i = 1; i <= n; i++) {
            for (int j = 1; j <= i; j++) {
                System.out.print("* ");
            }
            System.out.println();
        }
    }

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        StarPatterns sp = new StarPatterns();

        // Input for square
        System.out.print("Enter number of rows for square: ");
        int rows = sc.nextInt();

        System.out.print("Enter number of columns for square: ");
        int cols = sc.nextInt();

        // Input for triangle
        System.out.print("Enter height of triangle: ");
        int n = sc.nextInt();

        // Calling methods
        sp.square(rows, cols);
        sp.triangle(n);

        sc.close();
    }
}


Output:
<img width="443" height="330" alt="image" src="https://github.com/user-attachments/assets/d3233f75-b06c-44cc-a246-2820b730af34" />

# z
                                                Program-5

import java.util.Scanner;

class Distance {
    int meter;
    int cm;

    void input(int m, int c) {
        meter = m;
        cm = c;
    }

    Distance add(Distance d2) {
        Distance result = new Distance();
        result.cm = this.cm + d2.cm;
        result.meter = this.meter + d2.meter + (result.cm / 100);
        result.cm = result.cm % 100;
        return result;
    }

    void display() {
        System.out.println(meter + " m " + cm + " cm");
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        Distance d1 = new Distance();
        Distance d2 = new Distance();

        int m1 = sc.nextInt();
        int c1 = sc.nextInt();
        int m2 = sc.nextInt();
        int c2 = sc.nextInt();

        d1.input(m1, c1);
        d2.input(m2, c2);

        Distance result = d1.add(d2);

        result.display();

        sc.close();
    }
}
<img width="321" height="51" alt="image" src="https://github.com/user-attachments/assets/5e6f989a-0359-4e60-9654-5de37b460994" />

# a
                                                   Program-6

import java.util.Scanner;

class Distance {
    int meter, cm, mm;

    void input(int m, int c, int mi) {
        meter = m;
        cm = c;
        mm = mi;
    }

    Distance add(Distance d2) {
        Distance result = new Distance();

        result.mm = this.mm + d2.mm;
        result.cm = this.cm + d2.cm + (result.mm / 10);
        result.mm = result.mm % 10;

        result.meter = this.meter + d2.meter + (result.cm / 100);
        result.cm = result.cm % 100;

        return result;
    }

    void display() {
        System.out.println(meter + " m " + cm + " cm " + mm + " mm");
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        Distance d1 = new Distance();
        Distance d2 = new Distance();

        int m1 = sc.nextInt();
        int c1 = sc.nextInt();
        int mm1 = sc.nextInt();

        int m2 = sc.nextInt();
        int c2 = sc.nextInt();
        int mm2 = sc.nextInt();

        d1.input(m1, c1, mm1);
        d2.input(m2, c2, mm2);

        Distance result = d1.add(d2);

        result.display();

        sc.close();
    }
}

<img width="317" height="47" alt="image" src="https://github.com/user-attachments/assets/20cec896-006e-4ed4-8116-b7a8faa0b0f1" />

# b
                                                 Program-7

import java.util.Scanner;

class Time {
    int hr, min;

    void input(int h, int m) {
        hr = h;
        min = m;
    }

    Time add(Time t2) {
        Time result = new Time();

        result.min = this.min + t2.min;
        result.hr = this.hr + t2.hr + (result.min / 60);
        result.min = result.min % 60;

        return result;
    }

    void display() {
        System.out.println(hr + " hr " + min + " min");
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        Time t1 = new Time();
        Time t2 = new Time();

        int h1 = sc.nextInt();
        int m1 = sc.nextInt();

        int h2 = sc.nextInt();
        int m2 = sc.nextInt();

        t1.input(h1, m1);
        t2.input(h2, m2);

        Time result = t1.add(t2);

        result.display();

        sc.close();
    }
}

# b

<img width="306" height="52" alt="image" src="https://github.com/user-attachments/assets/2dd41f58-014a-4c1d-a8e9-1cb73b448811" />
