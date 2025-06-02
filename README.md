## Name : Raha Priya Dharshini M
## Reg no.:212224240124

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
int main()
{
unsigned int a=44 ; /* 60 = 0011 1100 */
int c;
c = a << 3; /* 240 = 1111 0000 */
printf("After Left Shift Operation value of a is:%d\n", c );
}
```


## OUTPUT

![image](https://github.com/user-attachments/assets/41665c55-3dd8-43c7-9d5e-c4a83ce41498)










## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


## AIM

Write a C Program to check whether the two numbers are equal or not using simple if statement.

## ALGORITHM

1.	Start the program.
2.	Read two numbers.
3.	If first number is equal to second number, display both are equal.
4.	Otherwise display both are not equal.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main()
{
   int m,n;
   scanf("%d",&m);
   scanf("%d",&n);
   if(m==n)
   {
     printf("Numbers are Equal");
   }
   else
   {
     printf("Numbers are not Equal");
    }
    return 0;
}
```


## OUTPUT

![image](https://github.com/user-attachments/assets/2a7725e0-ecfa-4088-8c8c-2ea609b77362)

           
## RESULT

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


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
#include<stdio.h>
#include<string.h>
#include<ctype.h>
int main()
{
    char a[10];
    scanf("%s",a);
    for(int i=0;a[i]!=0;i++)
    {
       a[i]=tolower(a[i]);
    }
    printf("Lower case String is:%s",a);
    return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/a1022a07-dcbc-447d-a828-21d0722e7068)





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
    char str[200];
    int i = 0, wordCount = 0;

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin); 

    if(str[strlen(str) - 1] == '\n') {
        str[strlen(str) - 1] = '\0';
    }

    do {
        
        if((i == 0 && str[i] != ' ') || 
           (str[i] != ' ' && str[i - 1] == ' ')) {
            wordCount++;
        }
        i++;
    } while(str[i] != '\0');

    printf("Total number of words: %d\n", wordCount);

    return 0;
}
```


## OUTPUT

![image](https://github.com/user-attachments/assets/0737f1b2-3e2d-44ec-856a-8fcbe0d54536)







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
#include <stdio.h>
#include <string.h>
int main()
{
   char str1[100], str2[100];
   int i;
   i = 0;
   scanf("%[^\n]%*c", str1);
   scanf("%[^\n]%*c", str2);
   do
   {
    if(str1[i]<str2[i])
    {
      printf("str1 is Less than str2");
      break;
    }
    else if(str1[i]>str2[i])
    {
       printf("str2 is Less than str1");
       break;
    }
    else
    {
       printf("str1 is Equal to str2");
    }
    }while(1);
         i++;
    return 0;
}
```


## OUTPUT
 
![image](https://github.com/user-attachments/assets/6219b3e0-9aa1-42e6-adaa-7fef2a1b7694)


## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

