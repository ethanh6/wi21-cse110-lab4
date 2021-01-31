1. What will happen at line 11 and why?
   - It outputs the length of the array. Since at last round of for loop, i would be incremented, which no longer satisfies the condition `i < prices.length`, so program quits the for loop. Mean while, i would hold the length of the array, since it's one more than the index of the last elememt. Additionally, declearation variable using `var` can ignore code block, thus it becomes global variable, available everywhere.

2. What will happen at line 12 and why?
   - It outputs the last value that `discountedPrice` holds, which is `[prices[prices.length-1] * (1-discount)`, since `discountedPrice` is decleared using var, thus can not be blocked by the scope of for loop.

3. What will happen at line 13 and why?
   - It outputs the last value holded by `finalPrice`, which is `Math.round(discountedPrice * 100) / 100`, since `finalPrice` is decleared inside the function `discountPrice`, it is accessible in the entire function. 

4. What will the function return if we call discountPrices([100, 200, 300], .5) ? Give a brief explanation.
   - It returns `[ 50, 100, 150]`. It's an array of prices (passed by parameter `prices`) with each element being multiplied by  `(1-discount)`.

<!-- ----- -->

5. What will happen at line 11 and why?
   - It throws an error with message "i is not defined", since `i` is decleared using `let`, its scope is limited to the for loop, thus not accessible outside the for loop.

6. What will happen at line 12 and why?
   - If line 11 is commented out, the program would throw an error with message "discountedPrice is not defined", since `discountedPrice` is decleared using `let`, its scope is limited to the for loop, thus not accessible outside the for loop.

7. What will happen at line 13 and why?
   - If line 11 and 12 are commented out, it outputs the value of `finalPrice`, which is `Math.round(discountedPrice * 100) / 100`, since this line is within the scope of `finalPrice`.

8. What will the function return for discountPrices([100, 200, 300], .5)? Give a brief explanation.
   - If line 11 and 12 are commented out, `discountPrices` would return an array of prices after applying `discount`; otherwise, the program would report error.

<!-- ----- -->

9. What will happen at line 11 and why?
    - The program will throw an error first since there's is a assignment to const variable.
    - If the assignment is sucessful at line 7, line 11 will throw another error (reference error) since i is declared using `let`, and `i` would be out of scope in line 11.

10. What will happen at line 12 and why?
    - If the assignement is successful at line 6 (which it shouldn't be), line 12 will throw a reference error: `discountedPrice` is not defined because `discountedPrice` is declared using const, and it would be out of scope at line 12.

11. What will happen at line 13 and why?
    - If the assignement is running successfully for all the lines above line 13, line 13 will print 0 because `finalPrice` is declared as a `const` and its value will not change.

12. What will the function return for discountPrices([100, 200, 300], .5)? Give a brief explanation.
    - If the assignement is running successfully, ignoring all errors, line 14 will return `[]` because `discounted` is declared as a `const` and its value will not change.

<!-- ----- -->
13.  
    -  A. student["name"]
    -  B. student["Grad Year"]
    -  C. student.greeting()
    -  D. student["Favorite Teacher"]["name"]
    -  E. student.courseLoad[0]

14.  
    -  A. '32'
       -  2 is converted to 2, then appended to 3
    -  B. 1
       -  3 is converted to Numver, then substracted by 2
    -  C. 3
       -  null is converted to 0, then added to 3
    -  D. '3null'
       -  null is converted to string, then appended to '3'
    -  E. 4
       -  true is converted to Number `1` then addede by 3
    -  F. 0
       -  both false and null are converted to 0
    -  G. '3undefined'
       -  undefined is converted to string and appended to '3'
    -  H. NaN
       -  "3" is converted to Number and undefined is converted to NaN, the resulf of addition is NaN
15.  
    -  A. true
       -  '2' is converted to Number and 2 > 1
    -  B. false
       -  The first char of both operand is '2' and '1', thus Boolean('2' < '12') is false by dictionary comparison.
    -  C. true
       -  '2' is converted to Number, thus Boolean(2==2) is true
    -  D. false
       -  `2` and `'2'` are of different, thus it's false
    -  E. false
       -  `true` is converted to 1, and 1 != 2
    -  F. true
       -  Boolean(2) is true, thus it's true

16.  `==` will convert two operands to have the same type before comparison; `===` is a more strict comparison operator where both value and type would be compared.

17.  The code would print "How are you?". For the first condition, `2 == true`, it converts `true` to `1`, thus the comparison is `false`.

18.  ans. in part1-question18.js

19.  In this case, `doSomething` is passed into `modifyArray` as a argument. 

- When execution, the for loop would be `newArr.push(doSomething(array[i], function (x) {return x*2}));`. `doSomething` would be called with first argument `array[i]` and second argument`function (x) {return x * 2}` (an anonymous function). 

- Inside `doSomething`, the anonymous function receives parameters `num + 2 and returns `(num + 2) * 2`.
 
-  Back to for loop, the program puts `newArr` the return value, `(num + 2) * 2`. So, with input `[1, 2, 3]`, the program outputs `[6, 8, 10]`.


20. part1-question20.js

21. 1 4 3 2  (in separate line)