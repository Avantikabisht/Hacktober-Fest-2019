# Hacktober Fest 2019
Hacktoberfest is a program by Digital Ocean, DEV and Github, where you can easily win a T-Shirt just by making 4 pull requests in the month of October to any open source projects on Github.

![image](https://user-images.githubusercontent.com/41102775/66319124-30589f00-e93a-11e9-9ff7-fdf03c09f9da.png)

# Steps to contribute.
1. Register for Hacktoberfest  https://hacktoberfest.digitalocean.com/
2. Fork this repository 
3. Add a Program in the specified folder of the language you like (if your language is not specified you can make that folder and then add your code in that folder)
4. Send a pull request and you are done with your first contribution!
5. Give this project a star if you liked working on it and share it as much as you can with people new to Open Source


# Happy Coding!!


// java program for Pascal's Triangle 
// A O(n^2) time and O(n^2) extra  
// space method for Pascal's Triangle 
import java.io.*; 
  
class PascalTriangle { 
    public static void main (String[] args) { 
        int n = 5; 
        printPascal(n); 
    } 
  
public static void printPascal(int n) 
{ 
// An auxiliary array to store generated pascal triangle values 
int[][] arr = new int[n][n];  
  
// Iterate through every line and print integer(s) in it 
for (int line = 0; line < n; line++) 
{ 
    // Every line has number of integers equal to line number 
    for (int i = 0; i <= line; i++) 
    { 
    // First and last values in every row are 1 
    if (line == i || i == 0) 
        arr[line][i] = 1; 
    else // Other values are sum of values just above and left of above 
        arr[line][i] = arr[line-1][i-1] + arr[line-1][i]; 
    System.out.print(arr[line][i]); 
    } 
    System.out.println(""); 
} 
} 
} 
