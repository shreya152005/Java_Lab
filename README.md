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

# c
                                                  Program-8
```
import java.util.Scanner;

class Time {
    int hr, min, sec;

    void input(int h, int m, int s) {
        hr = h;
        min = m;
        sec = s;
    }

    Time add(Time t2) {
        Time result = new Time();

        result.sec = this.sec + t2.sec;
        result.min = this.min + t2.min + (result.sec / 60);
        result.sec = result.sec % 60;

        result.hr = this.hr + t2.hr + (result.min / 60);
        result.min = result.min % 60;

        return result;
    }

    void display() {
        System.out.println(hr + " hr " + min + " min " + sec + " sec");
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        Time t1 = new Time();
        Time t2 = new Time();

        int h1 = sc.nextInt();
        int m1 = sc.nextInt();
        int s1 = sc.nextInt();

        int h2 = sc.nextInt();
        int m2 = sc.nextInt();
        int s2 = sc.nextInt();

        t1.input(h1, m1, s1);
        t2.input(h2, m2, s2);

        Time result = t1.add(t2);

        result.display();

        sc.close();
    }
}
```

Output:
<img width="235" height="51" alt="image" src="https://github.com/user-attachments/assets/e0865668-805c-482b-bf1a-3ab5f7b05f83" />

# d
                                                  Program-9

```
import java.util.Scanner;

class ArrayOperations {
    int[] arr;
    int size;

    void input() {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter size of array: ");
        size = sc.nextInt();
        arr = new int[size];

        System.out.println("Enter elements:");
        for (int i = 0; i < size; i++) {
            arr[i] = sc.nextInt();
        }
    }

    void output1() {
        System.out.println("Array elements:");
        for (int i = 0; i < size; i++) {
            System.out.print(arr[i] + " ");
        }
        System.out.println();
    }

    void output2() {
        System.out.println("Array using enhanced loop:");
        for (int x : arr) {
            System.out.print(x + " ");
        }
        System.out.println();
    }

    void reverse() {
        System.out.println("Array in reverse:");
        for (int i = size - 1; i >= 0; i--) {
            System.out.print(arr[i] + " ");
        }
        System.out.println();
    }
}

public class TestArray {
    public static void main(String[] args) {
        ArrayOperations obj = new ArrayOperations();

        obj.input();
        obj.output1();
        obj.output2();
        obj.reverse();
    }
}
```

Output:

<img width="337" height="143" alt="image" src="https://github.com/user-attachments/assets/f83f6243-d445-4c60-928b-e3c65a2671f4" />

# m
                                                      Program-10

```
import java.util.Scanner;

class MatrixOperations {
    int[][] a, b, result;
    int r, c;

    void input() {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter rows and columns: ");
        r = sc.nextInt();
        c = sc.nextInt();

        a = new int[r][c];
        b = new int[r][c];
        result = new int[r][c];

        System.out.println("Enter first matrix:");
        for (int i = 0; i < r; i++) {
            for (int j = 0; j < c; j++) {
                a[i][j] = sc.nextInt();
            }
        }

        System.out.println("Enter second matrix:");
        for (int i = 0; i < r; i++) {
            for (int j = 0; j < c; j++) {
                b[i][j] = sc.nextInt();
            }
        }
    }

    void addition() {
        System.out.println("Addition:");
        for (int i = 0; i < r; i++) {
            for (int j = 0; j < c; j++) {
                result[i][j] = a[i][j] + b[i][j];
                System.out.print(result[i][j] + " ");
            }
            System.out.println();
        }
    }

    void transpose() {
        System.out.println("Transpose of first matrix:");
        for (int i = 0; i < c; i++) {
            for (int j = 0; j < r; j++) {
                System.out.print(a[j][i] + " ");
            }
            System.out.println();
        }
    }

    void sumRows() {
        System.out.println("Sum of rows (first matrix):");
        for (int i = 0; i < r; i++) {
            int sum = 0;
            for (int j = 0; j < c; j++) {
                sum += a[i][j];
            }
            System.out.println(sum);
        }
    }

    void sumColumns() {
        System.out.println("Sum of columns (first matrix):");
        for (int i = 0; i < c; i++) {
            int sum = 0;
            for (int j = 0; j < r; j++) {
                sum += a[j][i];
            }
            System.out.println(sum);
        }
    }

    void sumDiagonal() {
        int sum = 0;
        for (int i = 0; i < r && i < c; i++) {
            sum += a[i][i];
        }
        System.out.println("Sum of diagonal (first matrix): " + sum);
    }
}

public class TestMatrix {
    public static void main(String[] args) {
        MatrixOperations obj = new MatrixOperations();

        obj.input();
        obj.addition();
        obj.transpose();
        obj.sumRows();
        obj.sumColumns();
        obj.sumDiagonal();
    }
}
```

Output:
<img width="329" height="326" alt="image" src="https://github.com/user-attachments/assets/6ffcddcc-34d3-4622-b8df-594358535497" />

# n

                                                  Program-11

```
//Without Thread (Sequential Execution)
class PrintTask1 {
    void printNumbers() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("Class 1: " + i);
        }
    }
}

class PrintTask2 {
    void printNumbers() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("Class 2: " + i);
        }
    }
}

class PrintTask3 {
    void printNumbers() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("Class 3: " + i);
        }
    }
}

public class SequentialDemo {
    public static void main(String[] args) {
        PrintTask1 t1 = new PrintTask1();
        PrintTask2 t2 = new PrintTask2();
        PrintTask3 t3 = new PrintTask3();

        t1.printNumbers();
        t2.printNumbers();
        t3.printNumbers();
    }
}

//With Thread Class
class ThreadTask1 extends Thread {
    public void run() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("Thread 1: " + i);
        }
    }
}

class ThreadTask2 extends Thread {
    public void run() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("Thread 2: " + i);
        }
    }
}

class ThreadTask3 extends Thread {
    public void run() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("Thread 3: " + i);
        }
    }
}

public class ThreadDemo {
    public static void main(String[] args) {
        ThreadTask1 t1 = new ThreadTask1();
        ThreadTask2 t2 = new ThreadTask2();
        ThreadTask3 t3 = new ThreadTask3();

        t1.start();
        t2.start();
        t3.start();
    }
}

//Using Runnable Interface
class RunnableTask1 implements Runnable {
    @Override
    public void run() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("Runnable 1: " + i);
        }
    }
}

class RunnableTask2 implements Runnable {
    @Override
    public void run() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("Runnable 2: " + i);
        }
    }
}

class RunnableTask3 implements Runnable {
    @Override
    public void run() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("Runnable 3: " + i);
        }
    }
}

public class RunnableDemo {
    public static void main(String[] args) {

        Thread t1 = new Thread(new RunnableTask1());
        Thread t2 = new Thread(new RunnableTask2());
        Thread t3 = new Thread(new RunnableTask3());

        t1.start();
        t2.start();
        t3.start();
    }
}
```

Output:

<img width="727" height="537" alt="image" src="https://github.com/user-attachments/assets/72c093ca-5a73-4ca8-9343-7f50cddeb517" />

<img width="684" height="539" alt="image" src="https://github.com/user-attachments/assets/f1162b89-8442-472f-a66e-c77b7e2e8abf" />

<img width="613" height="540" alt="image" src="https://github.com/user-attachments/assets/050cd7d0-72e6-4a2d-9762-cfed94ccbce9" />

<img width="699" height="536" alt="image" src="https://github.com/user-attachments/assets/60a94477-2b80-46d8-96c7-38abd3ea78ed" />

<img width="635" height="535" alt="image" src="https://github.com/user-attachments/assets/4f081b72-2058-4061-bf5a-8410c5f9e91d" />

<img width="575" height="536" alt="image" src="https://github.com/user-attachments/assets/a0619104-9d2f-444c-a5fd-e38600bb7423" />

<img width="657" height="535" alt="image" src="https://github.com/user-attachments/assets/cfe3ba8b-2a8c-43d7-8f28-a0fd245afef3" />

<img width="569" height="523" alt="image" src="https://github.com/user-attachments/assets/eb3edb10-120a-426e-b232-ba61d1e52ab4" />

<img width="583" height="531" alt="image" src="https://github.com/user-attachments/assets/f4f784e8-413a-40f9-a66d-16c74b75deaf" />

<img width="167" height="68" alt="image" src="https://github.com/user-attachments/assets/f65c5e92-0907-4927-85e8-f9de6ded8208" />

<img width="651" height="501" alt="image" src="https://github.com/user-attachments/assets/718790ab-2d38-4c96-936c-6248a0d80eac" />

<img width="670" height="537" alt="image" src="https://github.com/user-attachments/assets/c2410237-c21f-448c-bf3a-005675f5e411" />

# o
                                                  Program-12

```
class ThreadTask1 extends Thread {
    public void run() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("Thread 1: " + i);
        }
    }
}

class ThreadTask2 extends Thread {
    public void run() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("Thread 2: " + i);
        }
    }
}

class ThreadTask3 extends Thread {
    public void run() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("Thread 3: " + i);
        }
    }
}

public class JoinDemo {
    public static void main(String[] args) {

        ThreadTask1 t1 = new ThreadTask1();
        ThreadTask2 t2 = new ThreadTask2();
        ThreadTask3 t3 = new ThreadTask3();

        try {
            t1.start();
            t1.join();   // wait until Thread 1 completes

            t2.start();
            t2.join();   // wait until Thread 2 completes

            t3.start();
            t3.join();   // wait until Thread 3 completes

        } catch (InterruptedException e) {
            System.out.println(e);
        }

        System.out.println("All threads completed execution.");
    }
}
```

Output:
<img width="679" height="535" alt="image" src="https://github.com/user-attachments/assets/86af2622-eb7c-48b5-b08a-2c7e39431b01" />

# p
                                                  Program-13

```
import javax.swing.*;
import java.awt.event.*;

public class AddTwoNumbersSwing {

    public static void main(String[] args) {

        JFrame frame = new JFrame("Add Two Numbers");
        frame.setSize(400, 250);
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        frame.setLayout(null);

        JLabel l1 = new JLabel("Enter First Number:");
        l1.setBounds(50, 30, 150, 25);

        JLabel l2 = new JLabel("Enter Second Number:");
        l2.setBounds(50, 70, 150, 25);

        JLabel resultLabel = new JLabel("Result:");
        resultLabel.setBounds(50, 150, 300, 25);

        JTextField t1 = new JTextField();
        t1.setBounds(200, 30, 120, 25);

        JTextField t2 = new JTextField();
        t2.setBounds(200, 70, 120, 25);

        JButton addButton = new JButton("Add");
        addButton.setBounds(150, 110, 80, 30);

        addButton.addActionListener((ActionEvent e) -> {
            try {
                int num1 = Integer.parseInt(t1.getText());
                int num2 = Integer.parseInt(t2.getText());
                int sum = num1 + num2;
                resultLabel.setText("Result: " + sum);
            } catch (NumberFormatException ex) {
                resultLabel.setText("Please enter valid numbers!");
            }
        });

        frame.add(l1);
        frame.add(l2);
        frame.add(t1);
        frame.add(t2);
        frame.add(addButton);
        frame.add(resultLabel);

        frame.setVisible(true);
    }
}
```

Output:
<img width="348" height="221" alt="image" src="https://github.com/user-attachments/assets/db8e78fa-ca5f-42d1-9822-5e7af2d87488" />

# q
                                                  Program-14

```
import javax.swing.*;
import java.awt.event.*;

public class SwingCalculator {

    public static void main(String[] args) {

        JFrame frame = new JFrame("Calculator");
        frame.setSize(400, 300);
        frame.setLayout(null);
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);

        JTextField t1 = new JTextField();
        t1.setBounds(50, 30, 120, 30);

        JTextField t2 = new JTextField();
        t2.setBounds(200, 30, 120, 30);

        JButton add = new JButton("+");
        add.setBounds(50, 80, 60, 30);

        JButton sub = new JButton("-");
        sub.setBounds(120, 80, 60, 30);

        JButton mul = new JButton("*");
        mul.setBounds(190, 80, 60, 30);

        JButton div = new JButton("/");
        div.setBounds(260, 80, 60, 30);

        JLabel result = new JLabel("Result:");
        result.setBounds(50, 150, 300, 30);

        add.addActionListener((ActionEvent e) -> {
            double a = Double.parseDouble(t1.getText());
            double b = Double.parseDouble(t2.getText());
            result.setText("Result: " + (a + b));
        });

        sub.addActionListener((ActionEvent e) -> {
            double a = Double.parseDouble(t1.getText());
            double b = Double.parseDouble(t2.getText());
            result.setText("Result: " + (a - b));
        });

        mul.addActionListener((ActionEvent e) -> {
            double a = Double.parseDouble(t1.getText());
            double b = Double.parseDouble(t2.getText());
            result.setText("Result: " + (a * b));
        });

        div.addActionListener((ActionEvent e) -> {
            double a = Double.parseDouble(t1.getText());
            double b = Double.parseDouble(t2.getText());
            
            if (b != 0)
                result.setText("Result: " + (a / b));
            else
                result.setText("Cannot divide by zero");
        });

        frame.add(t1);
        frame.add(t2);
        frame.add(add);
        frame.add(sub);
        frame.add(mul);
        frame.add(div);
        frame.add(result);

        frame.setVisible(true);
    }
}
```

Output:
<img width="351" height="264" alt="image" src="https://github.com/user-attachments/assets/71dac235-b444-46e5-9d76-9a90f28aa6f8" />

# r
                                                  Program-15

```
import javax.swing.*;
import java.awt.event.*;

class MatrixAddFrame extends JFrame {

    JTextField a11, a12, a21, a22;
    JTextField b11, b12, b21, b22;
    JLabel result;

    MatrixAddFrame() {

        setTitle("Matrix Addition");
        setSize(500, 400);
        setLayout(null);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);

        a11 = new JTextField();
        a12 = new JTextField();
        a21 = new JTextField();
        a22 = new JTextField();

        b11 = new JTextField();
        b12 = new JTextField();
        b21 = new JTextField();
        b22 = new JTextField();

        JLabel l1 = new JLabel("Matrix A");
        l1.setBounds(50, 20, 100, 25);

        JLabel l2 = new JLabel("Matrix B");
        l2.setBounds(250, 20, 100, 25);

        a11.setBounds(50, 50, 50, 25);
        a12.setBounds(110, 50, 50, 25);
        a21.setBounds(50, 80, 50, 25);
        a22.setBounds(110, 80, 50, 25);

        b11.setBounds(250, 50, 50, 25);
        b12.setBounds(310, 50, 50, 25);
        b21.setBounds(250, 80, 50, 25);
        b22.setBounds(310, 80, 50, 25);

        JButton addBtn = new JButton("Add");
        addBtn.setBounds(180, 130, 100, 30);

        result = new JLabel("Result:");
        result.setBounds(50, 200, 400, 30);

        addBtn.addActionListener(new ActionListener() {
            public void actionPerformed(ActionEvent e) {

                int A[][] = new int[2][2];
                int B[][] = new int[2][2];
                int C[][] = new int[2][2];

                A[0][0] = Integer.parseInt(a11.getText());
                A[0][1] = Integer.parseInt(a12.getText());
                A[1][0] = Integer.parseInt(a21.getText());
                A[1][1] = Integer.parseInt(a22.getText());

                B[0][0] = Integer.parseInt(b11.getText());
                B[0][1] = Integer.parseInt(b12.getText());
                B[1][0] = Integer.parseInt(b21.getText());
                B[1][1] = Integer.parseInt(b22.getText());

                for (int i = 0; i < 2; i++) {
                    for (int j = 0; j < 2; j++) {
                        C[i][j] = A[i][j] + B[i][j];
                    }
                }

                result.setText("Result: [" + C[0][0] + " " + C[0][1] + "] [" + C[1][0] + " " + C[1][1] + "]");
            }
        });

        add(l1);
        add(l2);

        add(a11); add(a12); add(a21); add(a22);
        add(b11); add(b12); add(b21); add(b22);

        add(addBtn);
        add(result);

        setVisible(true);
    }
}

public class MatrixAdditionSwing {
    public static void main(String[] args) {
        new MatrixAddFrame();
    }
}
```

Output:

<img width="444" height="357" alt="image" src="https://github.com/user-attachments/assets/0c492d9d-3a10-49d9-aba4-0c59f3964bd3" />

# s
                                                  Program-16

import javax.swing.*;
import java.awt.*;
import java.awt.event.*;

public class ShapeDrawer extends JFrame implements ActionListener {

    private DrawPanel panel;

    public ShapeDrawer() {
        setTitle("Shape Drawer");
        setSize(800, 600);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        setLayout(new BorderLayout());

        // Drawing panel
        panel = new DrawPanel();
        add(panel, BorderLayout.CENTER);

        // Button panel
        JPanel buttonPanel = new JPanel();
        buttonPanel.setLayout(new GridLayout(2, 5, 5, 5));

        String[] buttons = {
                "Circle", "Oval", "Rectangle", "Square", "Line",
                "Triangle", "Arc", "RoundRect", "Polygon", "Star"
        };

        for (String text : buttons) {
            JButton btn = new JButton(text);
            btn.addActionListener(this);
            buttonPanel.add(btn);
        }

        add(buttonPanel, BorderLayout.SOUTH);

        setVisible(true);
    }

    @Override
    public void actionPerformed(ActionEvent e) {
        panel.setShape(e.getActionCommand());
    }

    // Drawing Panel
    class DrawPanel extends JPanel {

        private String shape = "";

        public void setShape(String shape) {
            this.shape = shape;
            repaint();
        }

        @Override
        protected void paintComponent(Graphics g) {
            super.paintComponent(g);

            g.setColor(Color.BLUE);

            switch (shape) {

                case "Circle":
                    g.drawOval(300, 100, 150, 150);
                    break;

                case "Oval":
                    g.drawOval(250, 120, 200, 120);
                    break;

                case "Rectangle":
                    g.drawRect(250, 100, 200, 120);
                    break;

                case "Square":
                    g.drawRect(300, 120, 150, 150);
                    break;

                case "Line":
                    g.drawLine(200, 200, 500, 200);
                    break;

                case "Triangle":
                    int[] tx = {300, 200, 400};
                    int[] ty = {100, 250, 250};
                    g.drawPolygon(tx, ty, 3);
                    break;

                case "Arc":
                    g.drawArc(250, 100, 200, 150, 0, 180);
                    break;

                case "RoundRect":
                    g.drawRoundRect(250, 120, 200, 120, 50, 50);
                    break;

                case "Polygon":
                    int[] px = {250, 300, 350, 400, 350, 300};
                    int[] py = {150, 100, 100, 150, 200, 200};
                    g.drawPolygon(px, py, 6);
                    break;

                case "Star":
                    int[] sx = {350, 370, 420, 380, 400, 350, 300, 320, 280, 330};
                    int[] sy = {100, 150, 150, 180, 230, 200, 230, 180, 150, 150};
                    g.drawPolygon(sx, sy, 10);
                    break;
            }
        }
    }

    public static void main(String[] args) {
        new ShapeDrawer();
    }
}


Output:

<img width="728" height="553" alt="image" src="https://github.com/user-attachments/assets/3a9b033d-85d7-4167-9727-2970d318af21" />

# t
                                                  Program-17

```
import javax.swing.*;
import java.awt.*;
import java.awt.event.*;
import java.util.ArrayList;

public class PaintBrush extends JFrame {

    private Color currentColor = Color.BLACK;
    private int brushSize = 5;

    public PaintBrush() {
        setTitle("Smooth Paint Brush");
        setSize(900, 600);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        setLayout(new BorderLayout());

        DrawArea drawArea = new DrawArea();
        add(drawArea, BorderLayout.CENTER);

        // Controls
        JPanel controls = new JPanel();

        JButton black = new JButton("Black");
        JButton red = new JButton("Red");
        JButton blue = new JButton("Blue");
        JButton green = new JButton("Green");

        black.addActionListener(e -> currentColor = Color.BLACK);
        red.addActionListener(e -> currentColor = Color.RED);
        blue.addActionListener(e -> currentColor = Color.BLUE);
        green.addActionListener(e -> currentColor = Color.GREEN);

        controls.add(black);
        controls.add(red);
        controls.add(blue);
        controls.add(green);

        JLabel label = new JLabel("Brush Size:");
        JSlider slider = new JSlider(1, 30, 5);

        slider.addChangeListener(e -> brushSize = slider.getValue());

        controls.add(label);
        controls.add(slider);

        add(controls, BorderLayout.SOUTH);

        setVisible(true);
    }

    // Line structure
    class Line {
        int x1, y1, x2, y2;
        Color color;
        int size;

        Line(int x1, int y1, int x2, int y2, Color color, int size) {
            this.x1 = x1;
            this.y1 = y1;
            this.x2 = x2;
            this.y2 = y2;
            this.color = color;
            this.size = size;
        }
    }

    class DrawArea extends JPanel {

        private java.util.List<Line> lines = new ArrayList<>();
        private int lastX, lastY;

        public DrawArea() {
            setBackground(Color.WHITE);

            addMouseListener(new MouseAdapter() {
                public void mousePressed(MouseEvent e) {
                    lastX = e.getX();
                    lastY = e.getY();
                }
            });

            addMouseMotionListener(new MouseMotionAdapter() {
                public void mouseDragged(MouseEvent e) {

                    int x = e.getX();
                    int y = e.getY();

                    lines.add(new Line(lastX, lastY, x, y, currentColor, brushSize));

                    lastX = x;
                    lastY = y;

                    repaint();
                }
            });
        }

        @Override
        protected void paintComponent(Graphics g) {
            super.paintComponent(g);

            Graphics2D g2 = (Graphics2D) g;

            for (Line line : lines) {
                g2.setColor(line.color);
                g2.setStroke(new BasicStroke(line.size, BasicStroke.CAP_ROUND, BasicStroke.JOIN_ROUND));
                g2.drawLine(line.x1, line.y1, line.x2, line.y2);
            }
        }
    }

    public static void main(String[] args) {
        new PaintBrush();
    }
}
```

Output:
<img width="825" height="548" alt="image" src="https://github.com/user-attachments/assets/d75b683b-f70a-430f-a061-3f595bc8e4c8" />

# v
                                                  Program-18
                                                  
```
package mypack;

public class Add {
    public int sum(int a, int b) {
        return a + b;
    }
}
package mypack;

public class Sub {
    public int subtract(int a, int b) {
        return a - b;
    }
}
package mypack;

public class Mul {
    public int multiply(int a, int b) {
        return a * b;
    }
}
package mypack;

public class Div {
    public int divide(int a, int b) {
        return a / b;
    }
}
package mypack;

public class Square {
    public int square(int a) {
        return a * a;
    }
}

//Main Method

import mypack.*;

public class Main {
    public static void main(String[] args) {
        Add a = new Add();
        Sub s = new Sub();
        Mul m = new Mul();
        Div d = new Div();
        Square sq = new Square();

        System.out.println("Addition: " + a.sum(10, 5));
        System.out.println("Subtraction: " + s.subtract(10, 5));
        System.out.println("Multiplication: " + m.multiply(10, 5));
        System.out.println("Division: " + d.divide(10, 5));
        System.out.println("Square: " + sq.square(5));
    }
}
```

Output:
<img width="362" height="87" alt="image" src="https://github.com/user-attachments/assets/119667ac-8748-4035-be0a-08040df2880b" />

# w
                                                  Program-19

```
package mypack;

public class Add {
    public int sum(int a, int b) {
        return a + b;
    }
}
package mypack.subpack;

public class Square {
    public int square(int a) {
        return a * a;
    }
}
import mypack.Add;
import mypack.subpack.Square;

//Main

public class Main {
    public static void main(String[] args) {

        Add a = new Add();
        Square s = new Square();

        System.out.println("Addition: " + a.sum(10, 5));
        System.out.println("Square: " + s.square(5));
    }
}
```

Output:
<img width="412" height="44" alt="image" src="https://github.com/user-attachments/assets/ed93a710-4d0d-4048-a86c-1111350d85cd" />

# e
                                                  Program-20

```
public class Main {
    public static void main(String[] args) {

        try {
            int arr[] = new int[5];

            arr[0] = 10;
            arr[1] = 20;
            arr[2] = 30;
            arr[3] = 40;
            arr[4] = 50;

            System.out.println("Accessing array elements:");
            for (int i = 0; i <= 5; i++) {  
                System.out.println("Element at index " + i + " = " + arr[i]);
            }

        } catch (ArrayIndexOutOfBoundsException e) {
            System. out.println("Array Index Out Of Bounds Exception caught!");
            System. out.println("You tried to access an invalid index in the array.");
        }

        try {
            int a = 10;
            int b = 0;

            int result = a / b;  
            System.out.println("Result = " + result);

        } catch (ArithmeticException e) {
            System. out.println("Arithmetic Exception caught!");
            System. out.println("Division by zero is not allowed.");
        }

        System.out.println("Program continues after handling exceptions.");
    }
}
```

Output:
<img width="384" height="182" alt="image" src="https://github.com/user-attachments/assets/1a2613fd-5fad-4d87-aebd-d5e50826f12c" />

# f
                                                  Program-21

```
class InvalidAgeException extends Exception {
    public InvalidAgeException(String message) {
        super(message);
    }
}

public class Main {

    static void checkAge(int age) throws InvalidAgeException {
        if (age < 18 || age > 25) {
            throw new InvalidAgeException("Age must be between 18 and 25.");
        } else {
            System. out.println("Valid age. Student allowed.");
        }
    }

    public static void main(String[] args) {

        int age = 16;  

        try {
            checkAge(age);
        } catch (InvalidAgeException e) {
            System. out.println("Exception caught: " + e.getMessage());
        }

        System.out.println("Program continues...");
    }
}
```

Output:
<img width="332" height="33" alt="image" src="https://github.com/user-attachments/assets/2b58d4d4-3680-4191-bf1a-70b22a56558d" />

