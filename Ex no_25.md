# EX 25 C program to check whether a given character is a vowel or consonant using pointer
## DATE:05/05/2025
## AIM:
To write a C program to check whether a given character is a vowel or consonant using pointer

## Algorithm
1. Start. 
2. Declare a variable value of type char. 
3. Prompt the user to enter a value. 
4. Read the value using scanf. 
5. Find vowel and consonants 
6. End.    

## Program:
```
#include <stdio.h> 
int main() { 
    char str[100]; 
    char *p; 
    int vowels = 0, consonants = 0; 
    scanf(" %[^\n]", str);   
    p = str;   
    while (*p != '\0') { 
        if ((*p >= 'A' && *p <= 'Z') || (*p >= 'a' && *p <= 'z')) { 
            char ch = (*p >= 'A' && *p <= 'Z') ? *p + 32 : *p; 
            if (ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u') { 
                vowels++; 
            } else { 
                consonants++; 
            } 
        } 
        p++; 
    } 
 
    printf("Vowels: %d\n", vowels); 
    printf("Consonants: %d\n", consonants); 
 
    return 0; 
}
```

## Output:
![image](https://github.com/user-attachments/assets/d6777e17-9bd8-4878-b9a8-5ecaf3b83e71)

## Result:
Thus the program was executed and the output was verified successfully.
