1. It outputs the length of the array. Since at last round of for loop, i would be incremented, which no longer satisfies the condition `i < prices.length`, so program quits the for loop. Mean while, i would hold the length of the array, since it's one more than the index of the last elememt. Additionally, declearation variable using `var` can ignore code block, thus it becomes global variable, available everywhere.
2. It outputs the last value that `discountedPrice` holds, since `discountedPrice` is decleared using var, thus can not be blocked by the scope of for loop.
3. It outputs the last value holded by `finalPrice`, since `finalPrice` is decleared inside the function `discountPrice`, it is accessible in the entire function. 
4. It returns `[ 50, 100, 150]`. It's an array of prices (passed by parameter `prices`) after applying `discount`.

<!-- ----- -->

5. It throws an error with message "i is not defined", since `i` is decleared using `let`, its scope is limited to the for loop, thus not accessible outside the for loop.

6. If line 11 is commented out, the program would throw an error with message "discountedPrice is not defined", since `discountedPrice` is decleared using `let`, its scope is limited to the for loop, thus not accessible outside the for loop.

7. If line 11 and 12 are commented out, it outputs the value of `finalPrice`, since this line is within the scope of `finalPrice`.

8. If line 11 and 12 are commented out, `discountPrices` would return an array of prices after applying `discount`; otherwise, the program would report error.

<!-- ----- -->

9. The program will first show an error at line 7 
10. adf
11. adsf
12. asdf
<!-- ----- -->
13. 
    1.  A. student["name"]
    2.  B. student["Grad Year"]
    3.  C. student.greeting()
    4.  D. student["Favorite Teacher"]["name"]
    5.  student.courseLoad[0]

14. 
    1.  A. '32'
    2.  B. 1
    3.  C. 3
    4.  D. '3null'
    5.  E. 4
    6.  F. 0
    7.  G. '3undefined'
    8.  H. NaN
15. 
    1.  A. true
    2.  B. false
    3.  C. true
    4.  D. false
    5.  E. false
    7.  F. 0
    8.  G. true

16. `==` will try to convert two operands to the same type, then compare the value; `===` will check the type and value of the two operands.