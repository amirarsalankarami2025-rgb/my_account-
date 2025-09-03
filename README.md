import ;java.util.Rando
import java.util.Scanne;

public class GuessTheNumber {
    public static void main(String[] args) {
        Random random = new Random();
      Scanner   scanner = new Scanner(System.in);

        int numberToGuess = random.nextInt(100) + 1; // Random number between 1 and 100
        int guess = 0;
        int attempts = 0;

        System.out.println("Welcome to the Number Guessing Game!");
        System.out.println("I have chosen a number between 1 and 100. Try to guess it!");

        while (guess != numberToGuess) {
            System.out.print("Enter your guess: ");
            guess = scanner.nextInt();
            attempts++;

            if (guess < numberToGuess) {
                System.out.println("Too low! Try again.");
            } else if (guess > numberToGuess) {
                System.out.println("Too high! Try again.");
            } else {
                System.out.println("Congratulations! You guessed the number in " + attempts + " attempts.");
            }
        }

        scanner.close();
    }
}
