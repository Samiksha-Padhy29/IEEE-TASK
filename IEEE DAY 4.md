//ARMSTRONG NUMBER  
\#include \<stdio.h\>  
\#include \<math.h\>  
\#include \<stdbool.h\>

bool isArmstrongNumber(int n) {  
    int original \= n, sum \= 0;  
    int digits \= log10(n) \+ 1;

    while (n \> 0\) {  
        int digit \= n % 10;  
        sum \+= pow(digit, digits);  
        n /= 10;  
    }

    return sum \== original;  
}  
//ANAGRAM CHECKER  
\#include \<stdio.h\>  
\#include \<string.h\>  
\#include \<stdbool.h\>

bool areAnagrams(char str1\[\], char str2\[\]) {  
    int freq\[256\] \= {0};

    for (int i \= 0; i \< strlen(str1); i++) {  
        freq\[(int)str1\[i\]\]++;  
    }

    for (int i \= 0; i \< strlen(str2); i++) {  
        freq\[(int)str2\[i\]\]--;  
    }

    for (int i \= 0; i \< 256; i++) {  
        if (freq\[i\] \!= 0\)  
            return false;  
    }

    return true;  
}  
//SUM OF EVEN NUMBER IN A LIST  
\#include \<stdio.h\>

int sumOfEvenNumbers(int arr\[\], int size) {  
    int sum \= 0;

    for (int i \= 0; i \< size; i++) {  
        if (\!(arr\[i\] & 1)) {  // Bitwise AND to check if the number is even  
            sum \+= arr\[i\];  
        }  
    }

    return sum;  
}  
//GCD  
\#include \<stdio.h\>

int gcd(int a, int b) {  
    while (b \!= 0\) {  
        int temp \= b;  
        b \= a % b;  
        a \= temp;  
    }  
    return a;  
}  
//CEL. TO FAR.  
\#include \<stdio.h\>

float celsiusToFahrenheit(float celsius) {  
    return ((celsius \* 1.8) \+ 32);  // Alternative formula representation  
}

