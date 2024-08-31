1. Difference between rem and em in css ?  
   em  \- It is related to that of closest parent element.  
   rem- It stands for root \- em it is always relative to that of font size of root element.   
     
2. Explain the concept of closures in JavaScript. Provide an example where a closure might be useful.(With code)?  
   Ans- It allows a function to access variables from its outer (enclosing) scope even after that outer function has finished executing.   
   function createCounter() {  
       let count \= 0;   
     
       return function() {  
           count \++;   
           return count;  
       };  
   }  
     
   const counter \= createCounter();  
     
   console.log(counter());   
3. What are semantic HTML tags?  
   Ans- Semantic HTML tags provide clear, descriptive meaning to elements, improving readability, accessibility, and SEO. Eg \- include header ,nav , main , aside  which convey specific roles and content structure.

       5\.  What is the purpose of the srcset attribute in the \<img\> tag?

Ans \- The `srcset` attribute in the `<img>` tag allows the browser to choose the best image based on the device’s screen size and resolution, optimizing performance and visual quality.

