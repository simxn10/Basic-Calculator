//# Basic-Calculator
//Calculator on Java Core

    import java.util.Scanner;
    import java.sql.SQLOutput;

    public class githubCalc {
    public static void main(String[] args){

        System.out.println(" pick your first value ");
        Scanner input = new Scanner(System.in);
        double num1 = input.nextDouble();

        System.out.println(" pick your second value ");
        Scanner input2 = new Scanner(System.in);
        double num2 = input2.nextDouble();

        System.out.println(" pick your action: addition, subtraction, multiplication, division ");
        Scanner inputFromSystem = new Scanner(System.in);
        String action = inputFromSystem.nextLine();

        if (action.equals ("addition")){
            double answer = num1 + num2;
            System.out.println("the answer is: "+answer);
        }

        else if (action.equals ("subtraction")){
            double answer = num1 - num2;
            System.out.println(" the answer is: "+answer);
        }

        else if (action.equals ("multiplication")){
            double answer = num1 * num2;
            System.out.println(" the answer is: "+answer);
        }

        else if (action.equals ("division")) {


            if (num2 == 0) {
                System.out.println(" your second value can not be 0");
            }

            else {
                System.out.println(" the answer is: " + (num1 / num2));
            }
        }

        else {
            System.out.println(" invalid input try again");
        }
        

       }
    }
