//PERFECT SQUARE  
\#include \<stdio.h\>

int isPerfectNumber(int num) {  
    int sum \= 0;  
    for(int i \= 1; i \<= num/2; i++) {  
        if(num % i \== 0\) {  
            sum \+= i;  
        }  
    }  
    return (sum \== num);  
}  
// PALLINDROME   
\#include \<stdio.h\>

int isPalindrome(int num) {  
    int originalNum \= num, reversedNum \= 0, remainder;  
      
    while(num \!= 0\) {  
        remainder \= num % 10;  
        reversedNum \= reversedNum \* 10 \+ remainder;  
        num /= 10;  
    }  
      
    return (originalNum \== reversedNum);  
}  
//COUNT VOWELS  
\#include \<stdio.h\>  
\#include \<ctype.h\>

int countVowels(const char \*str) {  
    int count \= 0;  
    char ch;  
      
    while (\*str \!= '\\0') {  
        ch \= tolower(\*str);  
        if (ch \== 'a' || ch \== 'e' || ch \== 'i' || ch \== 'o' || ch \== 'u') {  
            count++;  
        }  
        str++;  
    }  
      
    return count;  
}  
//REVERSE LIST  
\#include \<stdio.h\>

void reverseList(int arr\[\], int size) {  
    int temp;  
    for(int i \= 0; i \< size / 2; i++) {  
        temp \= arr\[i\];  
        arr\[i\] \= arr\[size \- 1 \- i\];  
        arr\[size \- 1 \- i\] \= temp;  
    }  
}  
//FACTORIAL OF A NUMBER  
\#include \<stdio.h\>

int factorial(int num) {  
    if(num \== 0 || num \== 1\) {  
        return 1;  
    } else {  
        return num \* factorial(num \- 1);  
    }  
}  
