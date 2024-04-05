Program to remove vowels from String
In this problem, we’re going to code a java Program to remove vowels from String. Take a string input from the user and store it in a variable called as “s” (in this case) .‘A’, ‘E’, ‘I’, ‘O’, ‘U’ are five vowels out of 26 characters in English alphabet letters.

Program to remove vowels
Algorithm
Take a String input from user and store is in a variable called as s 
After that take String variable s1 with empty String
After that call replaceAll() on s object 
Write regex on replaceAll() method like this s1 = s.replaceAll(“[aeiou]”, “”);
Print s variable
Note
Here we will use replaceAll() method to replace vowel from string the main work of replaceAll() method in java is to replace something by passing two arguments to this method i.e one is an old string and second is new string that you're replacing the old string with, so here we're passing a regular expression to replace vowels with blank spaces.
Code in Java
Run
import java.util.Scanner;

public class Main {

	public static void main(String[] args) {
		
        String s = "prepinsta";
        String s1 = "";
        s1 = s.replaceAll("[aeiou]", ""); 
        System.out.println("String after removing vowel : "+s1); 
	}

}

Output
String after removing vowel : prpnst
Method 2
We have used regex in this code.

Run
// Java program to remove vowels from a String
import java.util.Arrays;
import java.util.List;

class Main {
    static String remVowel(String str) {
        return str.replaceAll("[aeiouAEIOU]", "");
    }
    // Driver Code
    public static void main(String[] args) {
        String str = "Prepinsta";
        System.out.println(remVowel(str));
    }

}
Output
Prpnst
