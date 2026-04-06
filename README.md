package labact2;

import java.util.*;

public class gonzales2 {

	public static void main(String[] args) {

		int numbers[][] = { { 120, 250, 789, 7 }, { 58, 79, 31, 87 }, { 8, 1, 2, 3 }, { 99, 98, 97, 96 } };

		for (int i = 0; i < numbers.length; i++) {
			for (int j = 0; j < numbers[i].length; j++) {
				System.out.print(numbers[i][j] + "\t");
			}
			System.out.println();
		}

		for (int x = 0; x < numbers.length; x++) {
			for (int y = 0; y < numbers.length; y++) {
				if (numbers[x][y] == 1) {

					System.out.println("\nNumber 1 is found " + "at indices: " + x + " " + y + "\n");
				}
			}
		}

		for (int i = 0; i < numbers.length; i++) {
			for (int j = 0; j < numbers[i].length; j++) {
				if (numbers[i][j] == 1) {
					numbers[i][j] = 50;

				}
			}
		}
		for (int l = 0; l < numbers.length; l++) {
			for (int k = 0; k < numbers[l].length; k++) {
				System.out.print(numbers[l][k] + "\t");
			}
			System.out.println();
		}

		System.out.println("\n");
		
		for (int j = 0; j < numbers[1].length; j++) {
			for (int k = 0; k < numbers[j].length; k++) {
		    numbers[j][k] = 0;
		    System.out.print(numbers[j][k]+ "\t");
			}
		System.out.println();
		}
	}
	
}

