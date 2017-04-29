package com.company;
import java.util.Scanner;
public class Main {

    public static boolean isPrime(int num) {
        int countPrime=0;
        for (int i=1;i<=num;i++)
        {
            if (num%i==0){countPrime++;}
        }
        if (countPrime==2)
        {
            return true;
        }
        else
        {
            return false;
        }

    }

    public static boolean isPerfect(int num) {
        int ısPerfect=0;
        for (int i=1;i<num;i++){
            if (num%i==0)
            {
                ısPerfect=ısPerfect+i;
            }
        }
        if (ısPerfect==num)
        {
            return true;
        }
        else{
            return false;
        }
    }

    public static int factorize(int num, int[] factorArray) {
        int arrayLengt=0;
        for (int i=2;i<=num;i++)
        {
            while(num%i==0)
            {
                factorArray[arrayLengt]=i;
                num = num/i;
                arrayLengt++;
            }
        }
        return factorArray.length;
    }

    public static int findGCD(int num1, int num2) {
        int GCD=0,temp;
        if (num1<num2)
        {
            temp=num2;
        }
        else{
            temp=num1;
        }
        for (int i=1;i<=temp;i++)
        {
            if (num1%i==0&&num2%i==0)
            {
                GCD=i;
            }
        }
        return GCD;
    }

    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        System.out.println("Enter the number: ");
        int number = input.nextInt();

        if (isPrime(number))
            System.out.println(number + " is a prime number");
        else
            System.out.println(number + " is not a prime number");

        if (isPerfect(number))
            System.out.println(number + " is a perfect number");
        else
            System.out.println(number + " is not a perfect number");

        int[] fArray = new int[50];
        int numFactors = factorize(number, fArray);
        System.out.println("List of factors:");
        for (int i = 0; i < numFactors; i++)
        {
            if (fArray[i]!=0)
            System.out.println(fArray[i]);
        }

        System.out.println("\nEnter another number: ");
        int number2 = input.nextInt();
        System.out.println("The GCD of " + number + " and " + number2 + " is " + findGCD(number,number2));
    }
}
