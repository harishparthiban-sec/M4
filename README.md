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
int n=44;
printf("Value after left shift operation is %d",n<<3);
}
```
## OUTPUT
![alt text](image.png)








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
int main() {
int n,m;
scanf("%d%d",&m,&n);
if(m==n)
printf("Given numbers are equal");
else 
printf("Given numbers are not equal");
}
```

## OUTPUT
 ![alt text](image-1.png)   

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

#include <stdio.h>
int main() {
char str[10];
printf("Enter a string: ");
scanf("%[^\n]",str);
for(int i=0;str[i]!='\0';i++)
{
    if(str[i]>='A'&&str[i]<='Z')
    str[i]+=32;
}
printf("%s",str);
}
```
## OUTPUT
![alt text](image-2.png)



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
#include<ctype.h>
int main() {
char str[100];
int count=0;
printf("Enter a string: ");
scanf("%[^\n]",str);
for(int i=0;str[i]!='\0';i++)
{
    if(str[i]==' ')
    count++;
}
printf("Number of words = %d",count+1);
}
```
## OUTPUT
![alt text](image-3.png)




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
#include<ctype.h>
int main() {
char str1[100],str2[100];
int count=0;
printf("Enter a string 1: ");
scanf("%[^\n]",str1);
printf("Enter a string 2: ");
scanf(" %[^\n]",str2);
for(int i=0,j=0;(str1[i]!='\0'&&str2[j]!='\0');i++,j++)
{
    if(str1[i]!=str2[j])
    count++;
}
if(count==0)
printf("Given strings are same");
else
printf("Given strings are not same");
}
```

## OUTPUT
 ![alt text](image-4.png)

## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

