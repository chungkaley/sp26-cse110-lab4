1. The bug was a Data type error. The numbers that are entered into the input boxes are declared as string type. This means that using the + operator on the two string operands does not add them, but rather it joins them together. 
2. I would fix it by converting the strings into numbers before adding the operands. I would use the Number() function to wrap the operands. 
