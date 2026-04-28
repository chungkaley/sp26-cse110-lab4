1. Line 12 will print 3. This is because “i” is declared with var. Since var is function-scoped, this allows it to “leak” outside the loop. The loop iterates 3 times before exiting, so the final i++ would be 3. Hence, Line 12 will print 3. 
2. Line 13 will print 150. This is because discountPrice is declared with var. Since the var is function-scoped, this allows it to “leak outside the loop. The loop iterates 3 times before exiting, meaning that it uses the third element (300) in the array. 300 * (1-0.5) =150. Hence, Line 13 will print 150. 
3. Line 14 will print 150. The logic is the similar to #2. The finalPrice is declared with var, which is function-scoped. After the for loop exited, the code retains the third element (300) in the array.  300 * (1-0.5) = 150. Then, (150 x 100) /100 = 150. The value stored is the finalPrice and printed by Line 14. 
4. This function returns [50, 100, 150]. Each input price was discounted by 50%. Then, the code pushed the discounted prices into the discounted array during the loop. Hence, this returns [50, 100, 150] at the end of the function. 
5. Line 12 causes an error. This is because“i” is declared with let. Since let is blocked-scoped and only exists inside the for loop, it is not defined once the code reaches Line 12. 
6. Line 13 causes an error. This is similar to #5 as “discountedPrice” is declared with let. Since let is blocked-scoped and only exists inside the for loop, it is not defined once the code reaches Line 13.
7. Line 14 prints 150. The finalPrice is declared outside of the for loop. This means that finalPrice remains accessible after the for loop has executed. The finalPrice updates inside the loop. It holds the value from the last iteration and prints 150 on Line 14. 
8. This function returns [50, 100, 150]. The discounted array was declared outside of the for loop. This makes it accessible throughout the function. Hence, the loop was able to return the discounted values at Line 16.
9. Line 11 causes an error. The “i” is declared with let, which is block-scoped. This means that it is not defined when it is called on Line 11. 
10. Line 12 prints 3. The “length” is declared with const. This makes it accessible throughout the function. The variable “length” can only be read, so Line 12 can print the array length of 3. 
11. The function returns [50, 100, 150]. Even though “discounted” is declared with const, JavaScript allows the push() in the for loop to mutate the contents of an array as long as the code does not reassign the variable to a new array. 
12a. student.name

12b. student[‘Grad Year’]

12c. student.greeting()

12d. student[‘Favorite Teacher’].name

12e.studnet.courseLoad[0]

13a. The output is 32. The + operator joins operands together if the one of the operands is a string. 

13b. The output is 1. The - operator can be only used on numbers. The '3' is converted to a number. 

13c. The output is 3. The null is converted to 0 in numeric operations. 

13d. The output is 3null. The + operator joins operands together if the one of the operands is a string. 

13e. The output is 4. The true is converted to 1 in numeric operations. 

13f. The output is 0. The false and null are converted to 0 in numeric operations. 

13g. The output is 3undefined. The + operator joins operands together if the one of the operands is a string. 

13h. The output is NaN. The - triggers numeric operations and the undefined becomes NaN. 

14a. The output is true. The '2' is converted to 2 and compared to 1. 

14b. The output is false. With two strings, JavaScript uses lexicographical order. Since '2' comes after '1', '2' is considered greater than '1'.

14c. The output is true. The = = allows  '2' to be converted into the number 2. 

14d. The output is false The = = = does not allow '2' to be converted into the number 2.  

14e. The output is false. The true converts to 1. 1= =2 is false.

14f. The output is true. The Boolean(2) is true, meaning both are the same type and value. 

15. The = = operator allows the both values/operands to be converted to a common type through type coercion before comparing them. The = = = operator does not allow any conversion. If the value/operands ar different types, it returns false. 
