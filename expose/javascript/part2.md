1. Line 12 prints out `i` which has a value of 3. Line 12 prints out the value of the variable `i` which is of type var. Although `i` is declared within the for loop, since it is of type `var`, it can be accessed outside the for loop/elsewhere in the function. Line 12 is only accessed after the for loop terminates, meaning that `i = prices.length`. The length of prices is 3 so line 12 prints out 3.
2. Line 13 prints out the variable `discountedPrice` which is 150. `discountedPrice` is of type `var`, meaning it can be accessed outside the scope of the for loop where it is declared. The original purpose of `discountedPrice` is to calculate the discounted price of each value in the `prices` array and store it in the discounted array. After the loop terminates, the last discounted value within the `prices` array is stored within `discountedPrice` and remains accessible until the end of the function. The final value of the `prices` array is 300 and the discount is 0.5, meaning that the value of `discountedPrice` is 150. Line 13 then prints out that value.
3. Line 14 prints out the variable `finalPrice` which is 150. `finalPrice` is basically the same variable as `discountedPrice` but it is declared before the for loop and it accounts for how values of money can only have up to 2 numbers after the decimal. After the for loop terminates, `finalPrice` stores the discounted value of the last value inside `prices` which is 150. Since `finalPrice` is of type `var`, line 14 is able to access it without error. Line 14 then returns that value.
4. The function returns the `discounted` array which contains the values `[50, 100, 150]`. The `discountedPrices` function takes an array of values/prices and a discount value to apply to the array values. Since the discount value is `0.5`, the function returns an array of values that are all half of the values that were passed in.
5. The program returns an error as line 12 attempts to access a`i` which is of type let. `i`'s scope is limited to only the for loop since it is of type `let`, which line 12 is not a part of.
6. Same as above, the program returns an error as line 13 tries to access a variable that is out of scope. `discountedPrice` is a variable of type `let` that is declared within the for loop so line 13 returns an error since it is not within the loop.
7. Line 14 prints out `finalPrice` which has the value of 150. `finalPrice` is declared at the beginning of the function in the same code block as line 14 so line 14 has access to it. This is the same scenario as question 3 where  `finalPrice` is storing the discounted value of the last value of the `prices` array. Since the last value is 300 and the discount is 0.5, the resulting value is 150.
8. The function returns the `discounted` array which contains the values `[50, 100, 150]`. This is the same scenario as question 4, but with the type of variables being of type `let`. This causes no issues, however, as each variable is called within the appropriate scope. More specifically, `i` and `discountedPrice` are only called within the for loop. Same as quesiton 4, the starting values are reduced based on the discount value which is 0.5. So `[100, 200, 300]` becomes `[50, 100, 150]`.
9. Line 11 returns an error as `i` is of type of let, so it's only accessible within the for loop. Line 14 is after the for loop and thus returns an error because `i` can't be accessed.
10. Line 12 prints out `length` which is a `const` variable containing the value 3. `length = prices.length` and the length of prices is 3. Since `const` and `let` have the same scope accessibility and `length` is declared within the same scope as line 12, line 12 has access to it. Line 12 then prints out 3.
11. Same as question 4 and 8, the function returns an array with the values `[50, 100, 150]`. This time the function doesn't round off the decimals but the overall functionality is the same. Each variable is called within the appropriate scope. More specifically, `i` and `discountedPrice` are only called within the for loop. The starting values are reduced based on the discount value which is 0.5. So `[100, 200, 300]` becomes `[50, 100, 150]`. It also seems possible that `discounted` should cause an error since it is of type `const` and its values changes as it has values pushed into it. However, as long as you are mutating the array and not assigning it an entirely new array, that is allowed.
12. a) student.name;  
    b) student["Grad Year"];  
    c) student.greeting();  
    d) student["Favorite Teacher"].name;  
    e) student.courseLoad[0];  
13. a) '32': In javaScript, the + operation does concatenation if one or more of the operaters is a string.  
    b) 1: javScript converts string 3 to a number and performs the operation.  
    c) 3: javScript converts null to 0 since + is a mathematical operation.  
    d) '3null': Since 3 is a string, the plus operation becomes the string concatenation operation so null is treated as a string.  
    e) 4: Since 3 is a number, the + operation is treated numerically. True then gets converted to a number, which is 1.  
    f) 0: Both false and null are treated as numbers, both of which are converted to 0.  
    g) '3undefined': Since 3 is a string, + becomes the concatenation operation so undefined gets concatenated to 3.  
    h) NaN: String 3 is treated as a number because of the - operation. Undefined then gets converted to a NaN and 3 - NaN = NaN.  
14. a) true: String 2 gets converted to number 2.  
    b) false: Since both are strings, they do not get converted and are instead compared based on lexigraphical order.  
    c) true: string 2 is converted to number 2 because == allows for type conversion.  
    d) false: The === operator compares the types of the two operands first and returns false if they are different.  
    e) false: true is converted to number 1, which is not equal to 2.  
    f) true: The Boolean conversion converts any numerical value that isn't 0 into true.  
15. The `==` operator does type conversions before doing any operand comparison. The `===` operator checks the types of the operands and returns false if they are of different types. If they are of the same type, it then compares the operands values.
16. 
