## var declaration
### Question 1
What is printed by line 9? If the code returns an error, explain why. <br>
values added: 20

### Question 2
What is printed by line 13? If the code returns an error, explain why. <br>
final result: 20

### Question 3
Why should you not use var? Explain why. <br>
We shouldn't use var because it used to declare variables with function scope, which let the variable be accessed anywhere within the function it was defined in, regardless of the block it was defined in. By doing this, it can lead to naming conflicts and scoping issues in your programs, which is why it shouldn't be used. 

### Question 4
What is printed by line 9? If the code returns an error, explain why. <br>
values added: 20

### Question 5
What is printed by line 13? If the code returns an error, explain why. <br>
The code returns an error because let makes it so that result is limited to the scope of the block, but line 13 is out of the block.

## const declaration
### Question 6
What is printed by line 9? If the code returns an error, explain why. <br>
The code returns an error because result is a const, and const cannot be reassgiend after it is declared as 0.

### Question 7
What is printed by line 13? If the code returns an error, explain why. <br>
The code returns an error because result is a const and makes it so that there is an error in line 9. Because of that, it won't even reach line 13. 
