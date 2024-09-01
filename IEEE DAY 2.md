1.Write a function that checks if a given number is prime. A prime number is a number greater than 1 that has no divisors other than 1 and itself.  
 function checkPrime(num) {  
  let i, s=0;  
    for (i \= 2; i \<= num \- 1; i++) {  
        if (num % i \== 0\) {  
            c++;  
            break;  } }  
    if (s \== 2\)  console.log(" True");  
    else console.log(" False");}  
checkPrime(17);  
checkPrime(18);  
2.Write a function that checks if a given number is a strong number. A strong number is a number that is equal to the sum of factorials of the individual digits.  
function isStrongNumber(num) {  
  function factorial(n) {  
    if (n \=== 0 || n \=== 1\) return 1;  
    let result \= 1;  
    for (let i \= 2; i \<= n; i++) {  
      result \*= i;  
    }  
    return result;  
  }  
  const digits \= num.toString().split('');  
    const sumOfFactorials \= digits.reduce((sum, digit) \=\> sum \+ factorial(parseInt(digit)), 0);  
  return sumOfFactorials \=== num;  
}  
console.log(isStrongNumber(145));   
console.log(isStrongNumber(123));   
3\. Write a function that calculates the sum of all digits in a given integer.    
function sumOfDigits(num) {  
   let  a \=  0;  
    while(n\>0){  
        a \=a+ (n%10);  
        n= Number.parseInt(n/10);  
    }  
    return a;  
}  
console.log(sumOfDigits(12345));    
4\. Write a function that finds the maximum number in a given list of integers.  
function max(n){  
    let i,max;  
    for(i=1;i\<n.length;i++){  
if(n\[i-1\]\<n \[i\])   
max \= n\[i\]   
else  
 max \=n\[i-1\];  
    }  
    return max  
}  
let testNum \= \[1, 7, 3, 9, 2\];  
console.log(max(testNum));  
5.Write a function that takes a number as input and returns a list of Fibonacci numbers of length equal to that number.    
function Fibo(n){  
    let f \= \[0,1\];  
    if(n==1){  
        return f \[0\]  
    }  
    else if(n==2){  
        return f;  
    }  
    else{  
        let i,temp;  
        for(i \= 2 ; i\<n ; i++){  
            f.push(f \[i-1\] \+ f \[i-2\]); }   
        return f; }   
}  
console.log(Fibo(5));  
