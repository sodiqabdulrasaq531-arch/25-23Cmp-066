# 25-23Cmp-066
import java.util.Scanner;
public class HeronsFormula {
    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);

        // Input the three sides of the triangle
        System.out.print("Enter side a: ");
        double a = input.nextDouble();

        System.out.print("Enter side b: ");
        double b = input.nextDouble();

        System.out.print("Enter side c: ");
        double c = input.nextDouble();

        // Calculate semi-perimeter
        double s = (a + b + c) / 2;

        // Calculate area using Heron's formula
        double area = Math.sqrt(s * (s - a) * (s - b) * (s - c));

        // Display the result
        System.out.println("Semi-perimeter = " + s);
        System.out.println("Area of triangle = " + area);

        input.close();
    }
}