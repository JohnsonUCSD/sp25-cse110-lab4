## discountedPrices
1. It will print out "3" because `i` is a `var`, so it can be accessed anywhere in the function. There is a for loop just before line 12 and it gets incremented to 3, and that is what is being printed out
2. It will print out "150" because `discountedPrice` is a `var`, so it can be accessed anywhere in the function. In the for loop on line 7, the last time it is updated is on `i` = 2, so `discountedPrice` = (prices[2] * (1-0.5)) = (300 * 0.5) = 150.
3. It will print out "150" because `finalPrice` is a `var`, so it can be accessed anywhere in the function. In the for loop on line 8, the last time it is updated is on `i` = 2, so finalPrice = (Math.round(discountedPrice*100) / 100) = (Math.round(15000) / 100) = (15000/100) = 150.
4. The function returns [50, 100, 150] because `discounted` an array that gets pushed to in the for loop. The scope of it is in the function because is declared with `var`. The way we get those numbers for `discounted` is because the orignal array is [100, 200, 300] and the discount is 0.5, and the for loop applies this discount to all of the value in the original array and puts this new value into `discounted`, which is what gets returned.
5. It will return an error because by line 12, `i` is out of the scope. Because we declared `i` with `let` on line 6, which is in the for loop, it is only for inside the for loop, so because we are on line 12 now and out of the for loop, we are now out of the scope of `i` and will lead to an error.
6. It will return an error because by line 13, `discountedPrice` is out of the scope. Because we declared `discountedPrice` with `let` on line 7, which is in the for loop, it is only for inside the for loop, so because we are on line 13 now and out of the for loop, we are now out of the scope of `discountedPrice` and will lead to an error.
7. It will print out "150" because `finalPrice` is delcared with `let` on line 4 and the scope of it is within the function. Line 14 is still inside the scope of the function, so it will not result in an error unlike the previous 2 questions. In the for loop on line 8, the last time it is updated is on `i` = 2, so `finalPrice` = (Math.round(discountedPrice*100) / 100) = (Math.round(15000) / 100) = (15000/100) = 150.
8. The function returns [50, 100, 150] because `discounted` an array that gets pushed to in the for loop. The scope of it is in the function because is declared with `let` on line 3, which is in the function block. The way we get those numbers for `discounted` is because the orignal array is [100, 200, 300] and the discount is 0.5, and the for loop applies this discount to all of the value in the original array and puts this new value into `discounted`, which is what gets returned.
9. It will return an error because by line 11, `i` is out of the scope. Because we declared `i` with `let` on line 6, which is in the for loop, it is only for inside the for loop, so because we are on line 11 now and out of the for loop, we are now out of the scope of `i` and will lead to an error.
10. It will print out "3" because `length` is a `const` that was declared on line 4 and that is it. It will take the length of the pricecs, which is an array on three numbers, so when we do prices.length it is 3 and that is what `length` is assigned.
11. The function returns [50, 100, 150]. We are returning `discounted` which is a `const`, but since we are modifying it instead of reassigning it, it will not result in an error. The rest of the code is fine, so the function will work as normal and with the inputs, will return that answer.

## Data Types
12. 
- A. student.name
- B. student['Grad Year']
- C. student.greeting()
- D. student['Favorite Teacher'].name
- E. student.courseLoad[0]

## Basic Operators & Type Conversion 
13.  
- A. '32'
- B. 1
- C. 3
- D. '3null'
- E. 4 
- F. 0
- G. '3undefined'
- H. NaN
14.  
- A. true
- B. false
- C. true
- D. false
- E. false
- F. true
15. The difference between == and === is that == performs type conversion if the values have different types, while with === it doesn't do type conversion, so it needs both the same type and value.

## Functions
17. The function will return [2,4,6]. At the start we have an empty array `newArr`. We go into the for loop for the array in the input, [1,2,3], so it will go in the loop three times. In the loop, we are using the callback function, which we are inputting as doSomething, so it will do doSomething(array[i]) on line 4, and then push it into `newArr`. The doSomething function returns (num * 2) for the input given num. First is `i` = 0, so it will do doSomething(array[0]) = doSomething(1) = 1 * 2 = 2 and then it will push 2 into `newArr`. Next is `i` = 1, so it will do doSomething(array[1]) = doSomething(2) = 2 * 2 = 4 and then it will push 4 into `newArr`. Lastly, with `i` = 2, so it will do doSomething(array[2]) = doSomething(3) = 3 * 2 = 6 and then it will push 6 into `newArr`. After this for loop, it returns `newArr`, which we can see is [2,4,6] after everything is pushed. 

## setInterval(), setTimeout(), clearTimeout()
19. It will print out: <br>
1<br>
4<br>
3<br>
2<br>