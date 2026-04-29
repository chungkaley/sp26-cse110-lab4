1. 20
2. 20
3. You should not use var because var is function-scoped and can be declared below its use (known as hoisting). This can cause programmers to make errors such as naming conflicts, scoping issues, and making the code harder to read.  
4. 20 
5. The code returns an error because “let” is block-scoped. This means that result only exists within the curly brackets of the if statement. 
6. The code returns an error because “const” can not be reassigned.  
7. The code returns an error because “const” is block-scoped. This means that result only exists within the curly brackets of the if statement. Note: Line 7 would have returned an error because result is declared with const. 
