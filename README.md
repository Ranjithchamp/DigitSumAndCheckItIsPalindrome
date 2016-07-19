# DigitSumAndCheckItIsPalindrome
import java.util.Scanner;

public class DigitSumAndFindPalindrome {

	public static void main(String[] args) {
		int s = 0;
		int sum = 0;
		Scanner ww = new Scanner(System.in);
		System.out.println("enter a number");
		int q = ww.nextInt();
		while (q != 0) {
			sum += (q % 10);
			q = q / 10;
		}
		System.out.println("The sum of digits is"+sum);
		int ss = sum;
		int dumy = 0;

		while (sum != 0) {
			dumy = dumy * 10;
			dumy = dumy + (sum % 10);
			sum = sum / 10;

		}
		if (dumy == ss) {
			System.out.println("the sum of number is palindrome");
		} else {
			System.out.println("the sum is not palindrome");
		}

	}

}
