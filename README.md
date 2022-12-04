# 6-something
Write a program that prompts for and reads a year and also takes in an integer from 1-12 that corresponds to a month of the year. Use a switch statement to output the number of days in the month.

import java.util.Scanner
public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        int year, month, feb;
        
        feb = 29;
        System.out.println("Enter a year: ");
        year = scan.nextInt();
        System.out.println("Enter a month as 1-12: ");
        month = scan.nextInt();
       
        if (((year % 4 == 0) && (year % 100!= 0)) || (year%400 == 0))
            feb=29;
        else{
            feb=28;
        }
        
        System.out.println("Number of days in that month: ");
       
        switch(month){
            case 1:
                System.out.println("31");
                break;
            case 2:
                System.out.println(feb);
                break;
            case 3:
                System.out.println("31");
                break;
            case 4:
                System.out.println("30");
                break;
            case 5:
                System.out.println("31");
                break;
            case 6:
                System.out.println("30");
                break;
            case 7:
                System.out.println("31");
                break;
            case 8:
                System.out.println("31");
                break;
            case 9:
                System.out.println("30");
                break;
            case 10:
                System.out.println("31");
                break;
            case 11:
                System.out.println("30");
                break;
            case 12:
                System.out.println("31");
                break;
        }
    }
    
}
