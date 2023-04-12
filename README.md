import java.util.Scanner;

public class SkiSale {
  public static void main(String[] args) {
    Scanner scanner = new Scanner(System.in);

    System.out.println("Welcome to the Ski Sale!");
    System.out.println("What is your name?");

    String name = scanner.nextLine();

    System.out.println("Hi " + name + "! What kind of skis are you interested in?");
    System.out.println("1. Downhill skis");
    System.out.println("2. Cross-country skis");
    System.out.println("3. Snowboard");

    int choice = scanner.nextInt();

    switch (choice) {
      case 1:
        System.out.println("You have selected downhill skis.");
        System.out.println("These skis are 50% off today!");
        break;
      case 2:
        System.out.println("You have selected cross-country skis.");
        System.out.println("These skis are 40% off today!");
        break;
      case 3:
        System.out.println("You have selected a snowboard.");
        System.out.println("This snowboard is 30% off today!");
        break;
      default:
        System.out.println("Invalid choice.");
    }

    scanner.close();
  }
}
