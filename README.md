# Count-Vowels-and-Consonents-Java_interview_practice
package com.CountVowelConsonents;

import java.util.Scanner;

/**
 *
 * @author Dinesh Nanda
 */
public class CountVowelConsonents {

    public static void main(String[] args) {

        Scanner s = new Scanner(System.in);
        System.out.println("Enter a String: ");
        String st = s.nextLine();
        s.close();

        int vowels_count = 0, consonants_count = 0;

        for (int i = 0; i < st.length(); i++) {

            if (st.charAt(i) == ' ') {
                continue;
            } else if (st.charAt(i) == 'a' || st.charAt(i) == 'e' || st.charAt(i) == 'i' || st.charAt(i) == 'o' || st.charAt(i) == 'u'
                    || st.charAt(i) == 'A' || st.charAt(i) == 'E' || st.charAt(i) == 'I' || st.charAt(i) == 'O' || st.charAt(i) == 'U') {

                vowels_count++;
            } else {
                consonants_count++;
            }
        }
        System.out.println("Vowels: " + vowels_count + " and " + "Consonants: " + consonants_count);

    }

}
