# Fibonacci-Series

# Finding the nth number from Fibonacci Series taking user input

import java.util.Scanner;

class Fibonacci {

   public static void main(String args[]) {
   
        Scanner sc = new Scanner(System.in);
        System.out.println("Input the numbers: ");
        int n = sc.nextInt();
        
        int p = 0;
        int i = 1;
        int count = 2;

        while (count <= n) {
            int temp = i;
            i += p;
            p = temp;
            count++;
        }
        System.out.println("The " +n+" Fibonacci number is: " + i);
    }
}
