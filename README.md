import java.util.Scanner;

public class TriangleType {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Введіть першу сторону: ");
        double a = sc.nextDouble();

        System.out.print("Введіть другу сторону: ");
        double b = sc.nextDouble();

        System.out.print("Введіть третю сторону: ");
        double c = sc.nextDouble();
        
        if (a + b > c && a + c > b && b + c > a) {
            System.out.println("Трикутник існує.");
            
            if (a == b && b == c) {
                System.out.println("Трикутник рівносторонній.");
            } else if (a == b || a == c || b == c) {
                System.out.println("Трикутник рівнобедрений.");
            } else {
                System.out.println("Трикутник різносторонній.");
            }

        } else {
            System.out.println("Трикутник не існує.");
        }
    }
}
