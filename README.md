# Reverse

/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package reverse;
// Java program to Reverse a String using swapping
// of variables
import java.lang.*;
import java.io.*;
import java.util.*;
import java.util.Scanner;
 
// Class of ReverseString
class Reverse
{
    public static void main(String[] args)
    {
        Scanner reader = new Scanner(System.in);
        System.out.println("Enter some Text!: ");
        String input = reader.next();
        char[] temparray = input.toCharArray();
        int left, right=0;
        right = temparray.length-1;
 
        for (left=0; left < right ; left++ ,right--)
        {
            // Swap values of left and right
            char temp = temparray[left];
            temparray[left] = temparray[right];
            temparray[right]=temp;
        }
 
        for (char c : temparray){
            System.out.print(c);
        System.out.println();
        }
    }
}
