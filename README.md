# Sequence
Write a sequence with letters s for *, b for blank, n for new line and digit for times(x).


import java.util.Scanner;

//Image printer program

public class Pro3_1_150116011 {

	public static void main(String[] args) {
		
		Scanner input=new Scanner(System.in);
        String sequence;
        System.out.println("Please enter your sequence: ");
        sequence=input.nextLine();  //Getting the sequence from user
        int multiply=1; //This for digits in the sequence
        for(int i=0;i<sequence.length();i++){
            String character=sequence.substring(i, i+1);
           //Checking all characters one by one and sending to the switch-case.
        switch(character) {
        case "2":
        	multiply = 2;
        	break;
        case "3":
        	multiply = 3;
        	break;
        case "4":
        	multiply = 4;
        	break;
        case "5":
        	multiply = 5;
        	break;
        case "6":
        	multiply = 6;
        	break;
        case "7":
        	multiply = 7;
        	break;
        case "8":
        	multiply = 8;
        	break;
        case "9":
        	multiply = 9;
        	break; //From here we control the digits for how many characters should be printed.
        case "b":
        	for(int x = 1; x<=multiply; x++) {
        		System.out.print(" ");
        	}
        	multiply = 1;
        	break;
        case "s":
        	for(int x = 1; x<=multiply; x++) {
        		System.out.print("*");
        	}
        	multiply = 1;
        	break;
        case "n":
        	for(int x = 1; x<=multiply; x++) {
        		System.out.println();
        	}
        	multiply = 1;
        	break;
        } // Finally we control the characters and prints what it means.
        }
	}
}
