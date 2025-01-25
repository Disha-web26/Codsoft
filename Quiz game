import java.util.Scanner;
public class QuizApp {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        String[] questions = {
            "What is the capital of France? (a) Paris (b) London (c) Rome",
            "What is 5 + 3? (a) 8 (b) 10 (c) 12",
            "Who wrote 'Hamlet'? (a) Dickens (b) Shakespeare (c) Twain"
        };

        char[] answers = {'a', 'a', 'b'};
        int score = 0;

        for (int i = 0; i < questions.length; i++) {
            System.out.println(questions[i]);
            long startTime = System.currentTimeMillis();

            System.out.print("Your answer: ");
            char userAnswer = scanner.next().charAt(0);

            long endTime = System.currentTimeMillis();
            if ((endTime - startTime) > 10000) { // 10 seconds
                System.out.println("Time is up!");
            } else if (userAnswer == answers[i]) {
                System.out.println("Correct!");
                score++;
            } else {
                System.out.println("Wrong!");
            }
        }

        System.out.println("\nYour score: " + score);
        scanner.close();
    }
}


