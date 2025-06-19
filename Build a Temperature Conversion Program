import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Prompt user for temperature input
        System.out.print("Enter temperature value: ");
        double temp = scanner.nextDouble();

        // Prompt user for temperature unit
        System.out.print("Enter unit (C for Celsius, F for Fahrenheit, K for Kelvin): ");
        char unit = scanner.next().toUpperCase().charAt(0);

        double celsius = 0, fahrenheit = 0, kelvin = 0;

        switch (unit) {
            case 'C':
                celsius = temp;
                fahrenheit = (celsius * 9/5) + 32;
                kelvin = celsius + 273.15;
                break;
            case 'F':
                fahrenheit = temp;
                celsius = (fahrenheit - 32) * 5/9;
                kelvin = celsius + 273.15;
                break;
            case 'K':
                kelvin = temp;
                celsius = kelvin - 273.15;
                fahrenheit = (celsius * 9/5) + 32;
                break;
            default:
                System.out.println("Invalid unit entered. Please use C, F, or K.");
                return;
        }

        // Display results
        System.out.printf("Celsius: %.2f°C\n", celsius);
        System.out.printf("Fahrenheit: %.2f°F\n", fahrenheit);
        System.out.printf("Kelvin: %.2fK\n", kelvin);

        scanner.close();
    }
}
