# rockpaperscissors
Rock paper and scissors with computer using Java
import java.util.Scanner;
import java.util.Random;

public class ques_3 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        //0 for rock
        // 1 for scissors
        // 2 for paper
        System.out.println("Enter 0 for rock, 1 for scissors, 2 for paper");
        int userInput = sc.nextInt();

        Random rand = new Random();
        int compInput = rand.nextInt(3);
        System.out.println("computer choice " + compInput );
        
        if (compInput == userInput){
            System.out.println("Draw");
        }
        else if (userInput == 0 && compInput == 2 || userInput == 1 && compInput == 0
                || userInput == 2 && compInput == 1) {

            System.out.println("You Win!");
        }
        else {
            System.out.println("computer wins");
        }



    }
}
