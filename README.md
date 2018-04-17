# Summary
import java.util.Scanner;

import java.util.Random;
import java.util.Arrays;

public class Binary {

	public static void main(String[] args) {
	long time = System.currentTimeMillis();
	System.out.println(time);
		Scanner in = new Scanner(System.in);
		
		/*short inputNumber = in.nextShort(); //get number by user input
		for (int i = 128; i > 0; i/=2 ) {
			if (inputNumber >=i) {
				System.out.print("1");
				inputNumber -=i;
			}
			else {
				System.out.print("0");
			} //end for this loop
		}*/
		
		
		int arr[] = new int[8];
		for(int i = 0 ; i < arr.length; i++) {
			arr[i] = i*2;
		
		}
		for(int l : arr)System.out.println(l);// for each loop
		Arrays.sort(arr);//Quick Sort Algorithm
		long timeNow = System.currentTimeMillis();
		long duration = timeNow - time;
		System.out.println("Duration of the program "+duration +"ms");
	}
	public static void isNumberOdd (int number) {
		if (number%2==1) {
			System.out.println("The number is odd");
		}
		else {
			System.out.println("The number isn't even");
		}
	}
	public static void isRandomNumber (int inputRandomNumber) {
		Random rand = new Random (System.currentTimeMillis()); //Seed random function
		long timeNow = System.currentTimeMillis();
		System.out.print("Current Time in milliseconds = " + timeNow); // returns the current time in milliseconds
	}
	
}
