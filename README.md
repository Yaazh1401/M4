# EX-16-LEFT-SHIFT-OPERATION
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int a = 44;
    int shift = 3;
    int result = a << shift;
    printf("After Left Shift Operation value of a is:%d\n", result);
    
    return 0;
}
```
## OUTPUT

![image](https://github.com/user-attachments/assets/f4322fc0-7f28-4cac-953d-36d5a816dc88)








## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


## AIM

C program to check even or odd number using bitwise operator using if else

## ALGORITHM

1.	Start the program.
2.	Read a numbers.
3.	Check the least significant bit of a using the bitwise AND operator (a & 1):
    If the result is 1, then:
    Print "a is odd."
    Else:
    Print "a is even."
4.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    if(a & 1)
    {
        printf("%d is odd.",a);
    }
    else
    {
        printf("%d is even.",a);
    }
    return 0;
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/1c536fe6-8525-4273-a774-cf5d5167968b)
     
## RESULT

Thus the program to check whether the number is odd or  not using if else statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <ctype.h>

int main() {
    char str[100];
    scanf("%s", str); 
    for (int i = 0; str[i] != '\0'; i++) {
        str[i] = tolower(str[i]);
    }
    printf("Lower case String is: %s\n", str);
    return 0;
}

```
## OUTPUT

![image](https://github.com/user-attachments/assets/12d71c9e-3238-4438-b995-81cdce13e275)



## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <string.h>
int main() {
    char str[100];
    int i, word_count = 0;
    scanf(" %[^\n]", str); 
    for (i = 0; str[i] != '\0'; i++) {
        if (str[i] == ' ' && str[i+1] != ' ' && str[i+1] != '\0') {
            word_count++;
        }
    }
    if (str[0] != '\0')
        word_count++;
    printf("%d\n", word_count);
    return 0;
}

```
## OUTPUT
![image](https://github.com/user-attachments/assets/559e7051-ea08-4289-9192-05fa3e8bca53)





## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
Step 1: Start the program.
Step 2: Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variable
             flag and initialize it to 0, and i for indexing.      
Step 3: Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered 
            (i.e., can include spaces).
Step 4: Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no 
            spaces in the second string).
Step 5: Start comparing characters of both strings from index i = 0.
Step 6: Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string):
•	If c1[i] is not equal to c2[i], set flag = 1.
•	Increment i by 1.
Step 7: After the loop, check the value of flag:
•	If flag == 0, print "strings are same".
•	Otherwise, print "strings are not same".
Step 8: End the program.

## PROGRAM
```
#include<stdio.h>
#include<string.h>  
int main()  
{  
   char str1[20]; 
   char str2[20];  
   int value;
   scanf("%s",str1);  
   scanf("%s",str2) ;
   value=strcmp(str1,str2);  
   if(value==0) 
   {
   printf("strings are same");  
   }
   else  
   {
   printf("strings are not same");  
   }
   return 0;  
}    
```

## OUTPUT
 ![image](https://github.com/user-attachments/assets/4d0d4293-428b-4d53-a7a2-5b594b579164)


## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

