1. Because the 'i' variable was initialized using the var keyword, it can still be accessed outside of the for loop. On line 12, the most recent value of 'i', 3, is printed.
2. Because the 'discountedPrice' variable was initialized using the var keyword, it can still be accessed outside of the for loop. On line 13, the most recent value of 'discountedPrice', 150, is printed.
3. Because the 'finalPrice' variable was initialized using the var keyword, it can be accessed inside of the 'discountPrices' function. On line 14, the most recent value of 'finalPrice', 150, is printed.
4. This function will return an array of integers, [50, 100, 150], because the for loop is pushing the new prices to the array after the discount is applied in each iteration.
5. A reference error is returned at line 12 because the 'i' variable was initialized using the let keyword, which means it can only be accessed within the block it is defined in. In this situation, the 'i' variable is only accessible in the for loop.
6. A reference error is returned at line 13 because the 'discountedPrice' variable was initialized using the let keyword, which means it can only be accessed within the block it is defined in. In this situation, the 'discountedPrice' variable is only accessible in the for loop.
7. 150 is printed at line 14 because the 'finalPrice' variable was initialized using the let keyword, which means it is accessible within the block it is defined in. In this situation, 'finalPrice' was initialized at the beginning of the function and outside of the for loop, so we can access the variable at line 14.
8. This function will return an array of integers, [50, 100, 150], because the for loop is pushing the new prices to the array after the discount is applied in each iteration.
9. A reference error is returned at line 11 because the 'i' variable was initialized using the let keyword, which means it can only be accessed within the block it is defined in. In this situation, the 'i' variable is only accessible in the for loop.
10. 3 is printed at line 12 because the 'length' variable was initialized using the const keyword, which has the same scope as the let keyword. In addition, the 'length' variable was never reassigned.
11. This function will return an array of integers, [50, 100, 150], because the for loop is pushing the discounted prices to the array after they are calculated in each iteration.
12. A. student['name']
    
    B. student['Grad Year']

    C. student.greeting()

    D. student['Favorite Teacher']['name']

    E. student['courseLoad'][0]
13. A. '32' is outputted because the integer value of 2 is concatenated to the string value of '3'.
    
    B. 1 is outputted because numeric conversion happens in mathematical functions and expressions automatically. The subtraction expression is strictly a mathematical expression, so the string value of '3' is converted to an integer.

    C. 3 is outputted because null is automatically converted to 0 in mathematical functions and expressions. Thus, we have 3 + 0, which is equal to 3.

    D. '3null' is outputted because null is automatically converted to a string in string concatenation.

    E. 4 is outputted because true is automatically converted to 1 in mathematical functions and expressions. Thus, we have 1 + 3, which is equal to 4.

    F. 0 is outputted because false is automatically converted to 0 and null is automatically converted to 0 in mathematical functions and expressions. Thus, we have 0 + 0, which is equal to 0.

    G. '3undefined' is outputted because undefined is automatically converted to a string in string concatenation.

    H. NaN is outputted because '3' is converted to 3 and undefined is converted to NaN in mathematical functions and expressions. Thus, we have 3 - NaN, which is equal to NaN.
14. A. true is outputted because JavaScript converts values to numbers when comparing values of different types. Thus, '2' is converted to 2 in the comparison of '2' > 1, and 2 is greater than 1.
    
    B. false is outputted because JavaScript uses lexicographical order when comparing strings. Because '12' occurs before '2' in lexicographical order, the statement '2' < '12' is false.

    C. true is outputted because JavaScript converts values to numbers when comparing values of different types, and the strict equality operator is not used in this situation. Thus, '2' is converted to 2 in the statement 2 == '2'.

    D. false is outputted because the strict equality operator is used here, which means that equality is checked without type conversion. Thus, '2' is not converted to 2 in the statement 2 === '2', and false is outputted because the values are different types.

    E. false is outputted because JavaScript converts values to numbers when comparing values of different types. Thus, true is converted to 1 in the statment true == 2, and 1 is not equal to 2.

    F. true is outputted because Boolean(2) evaluates to true because 2 is not an "intuitively" empty value. Thus, we have true === true.
15. The == operator converts operands of different types to numbers before checking for equality while the === operator does not do any type conversion before checking for equality of operands.
17. When the function is called with the following parameters **modifyArray([1, 2, 3], doSomething)**, the function will return [2, 4, 6]. This is because we are passing in the doSomething function as a callback function in the modifyArray function, which makes the doSomething function callable within the modifyArray function. Therefore, the doSomething function is called on each element in [1, 2, 3] before they are pushed to a new array.
19. The code prints out 1, 4, 3, 2 on separate lines and in that order. Although the timeout on line 4 is set to 0, 4 is printed before 3 because setTimeout places the code on a queue and schedules it to run at the next opportunity. Currently-executing code must complete before functions on the queue are executed, thus 4 is printed before 3. 2 is printed last because it has a timeout of 1000 milliseconds.