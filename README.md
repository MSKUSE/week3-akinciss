public class FindGrade {

    public static void main(String[] args) {

        int score = Integer.parseInt(args[0]);

        if (score >= 90 ){
            System.out.println("Grade :A");

        } else if (score >= 80 && score <=89) {
            System.out.println("Grade :B");

        } else if (score>=70 && score <=79) {
            System.out.println("Grade :C");

        } else if (score >=60 && score <=69) {
            System.out.println("Grade : D");

        }else {
            System.out.println("Grade :F");
        }
    }
}
public class FindMaximum {
    public static void main(String[] args) {

        int num1=Integer.parseInt(args[0]);
        int num2=Integer.parseInt(args[1]);

        boolean condition = num1>num2;
        int max = condition ? num1 : num2;

        System.out.println(max);


    }
}
public class FindMinimum {

    public static void main(String[] args) {
        int num1 = Integer.parseInt(args[0]);
        int num2= Integer.parseInt(args[1]);
        int num3 = Integer.parseInt(args[2]);

        boolean num1_min = num1 < num2 && num1 < num3;
        boolean num2_min = num2 < num1 && num2 <num3;

        int min = num1_min ? num1 : num2_min ? num2 :num3;
        System.out.println(min);

    }
}
public class FindPrimes {
    public static void main(String[] args) {
        int number = Integer.parseInt(args[0]);

        for (int i = 0; i <= number; i++) {
            boolean isPrime = true;
            for (int j = 2; j < i; j++) {
                if (i % j ==0){
                    isPrime = false;
                    break;
                }
                if(isPrime){
                    System.out.println(i);
                }
                
            }

        }

    }
}
