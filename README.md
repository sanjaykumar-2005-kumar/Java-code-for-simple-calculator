# Experiment 01: Simple Calculator Using Java

## Aim
To develop a simple calculator using Java to perform basic arithmetic operations such as addition, subtraction, multiplication and division.

## Software Required
- Java JDK
- VS Code

## Description
This program performs basic arithmetic operations based on user input. It uses the Scanner class to get input and a switch statement to select the operation.

## Algorithm
1. Start the program.
2. Import the Scanner class.
3. Get two numbers from the user.
4. Get the arithmetic operator.
5. Use switch case to perform the operation.
6. Display the result.
7. Stop the program.

## Source Code

```java
import java.util.Scanner;

public class Calculator {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter first number: ");
        int a = sc.nextInt();

        System.out.print("Enter second number: ");
        int b = sc.nextInt();

        System.out.print("Enter operator (+, -, *, /): ");
        char op = sc.next().charAt(0);

        switch(op) {
            case '+':
                System.out.println("Addition = " + (a+b));
                break;

            case '-':
                System.out.println("Subtraction = " + (a-b));
                break;

            case '*':
                System.out.println("Multiplication = " + (a*b));
                break;

            case '/':
                if(b != 0)
                    System.out.println("Division = " + (a/b));
                else
                    System.out.println("Cannot divide by zero");
                break;

            default:
                System.out.println("Invalid Operator");
        }

        sc.close();
    }
}
```

## Output

```text
Enter first number: 20
Enter second number: 10
Enter operator (+, -, *, /): +
Addition = 30
```

## Result
Thus, the Java program for a simple calculator was successfully executed using arithmetic operators and switch statements.
