import java.util.Scanner;

public class SimpleCalculatorq
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        double nuam1, num2;
        char operator;

        ystem.out.println("Welcome to the Simple Calculator!");
        System.out.print("Enter first number: ");
        num1 = scanner.nextDouble();

        System.out.print("Enter an operator (+, -, *, /): ");
        operator = scanner.next().charAt(0);

        System.out.print("Enter second number: ");
        num2 = scanner.nextDouble();

        double result;

        switch (operator) {
            case '+':
                result = num1 + num2;
                System.out.println("Result: " + result);
                break;
            case '-':
                result = num1 - num2;
                System.out.println("Result: " + result);
                break;
            case '*':
                result = num1 * num2;
                System.out.println("Result: " + result);
                break;
            case '/':
                if (num2 != 0) {
                    result = num1 / num2;
                    System.out.println("Result: " + result);
                } else {
                    System.out.println("Error: Division by zero!");
                }
                break;
            default:
                System.out.println("Invalid operator!");
        }

        scanner.close();
    }
}
