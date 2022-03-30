# Angry-Professer
Hackerrank Problem Solution in Java
import java.util.Iterator;
import java.util.Scanner;

public class AngryProfessor {

	public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        int t = scan.nextInt();
        for (int i = 0; i < t; i++) {
			
		int n = scan.nextInt();
		int k = scan.nextInt();
		int ar[] = new int[n];
		for (int j = 0; j < ar.length; j++) {
			ar[j] = scan.nextInt();
		}
		int count = 0;
		for (int l = 0; l < ar.length; l++) {
			if(ar[l] <= 0) {
				count++;
			}
		}
		if(count < k) {
			System.out.println("YES");
		}
		else {
			System.out.println("NO");
		}
        }
	}

}
