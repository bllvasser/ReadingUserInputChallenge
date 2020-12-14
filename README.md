# ReadingUserInputChallenge
package academy.learnprogrmming;

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        int counter = 0;
        int sum = 0;

        while(counter < 10) {
            int order = counter + 1;
            System.out.println("Enter number #" + order + ":");

            boolean isAnInt = scanner.hasNextInt();

            if(isAnInt) {
                int number = scanner.nextInt();
                counter ++;
                sum += number;
            } else {
                System.out.println("Invalid number");
            }
            scanner.nextLine();
        }
        System.out.println("Sum = " + sum);

        scanner.close();

    }
}
"C:\Program Files\Java\jdk-15.0.1\bin\java.exe" "-javaagent:C:\Users\nadiy\OneDrive\Desktop\IntelliJ IDEA Community Edition 2020.2.3\lib\idea_rt.jar=50367:C:\Users\nadiy\OneDrive\Desktop\IntelliJ IDEA Community Edition 2020.2.3\bin" -Dfile.encoding=UTF-8 -classpath C:\Users\nadiy\IdeaProjects\ReadingUserInputChallenge\out\production\ReadingUserInputChallenge academy.learnprogrmming.Main
Enter number #1:
10
Enter number #2:
abc
Invalid number
Enter number #2:
def
Invalid number
Enter number #2:
20
Enter number #3:
30
Enter number #4:
40
Enter number #5:
50
Enter number #6:
60
Enter number #7:
70
Enter number #8:
80
Enter number #9:
90
Enter number #10:
100
Sum = 550

Process finished with exit code 0
