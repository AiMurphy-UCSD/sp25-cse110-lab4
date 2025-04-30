
1) At line 12, it will print "3" because the i in the for loop is a var, so it takes on the scope of the entire function, and it is 3 by the time it exits the for loop
2) At line 13, it will print "150" because discountedPrice was a declared a var in the for loop, therefore it has the scope of the entire function and can be accessed outside the for loop
3) At line 14, it will print "150" because finalPrice was a declared a var, therefore it has the scope of the entire function, it gets updated while in the for loop which is how it gets its value of 150
4) The function will return the array of discounted prices, [50, 100, 150], because the function has a return statement which returns discounted, which is an empty array at the start of the function, and gets the discounted prices added to it throughout the for loop, and with a discount of .5, 100 becomes 50, 200 becomes 100 and 300 becomes 150
5) At line 12, it will throw a ReferenceError, as i is declared with let, its scope is only inside the for loop, so outside the for loop it is not defined
6) At line 13, it will throw a ReferenceError, as discountedPrice is delcared with let within the for loop, which means its scope is only the for loop, so it is not defined outside the for loop
7) At line 14, it will print "150" as the variable finalPrice is declared using let, meaning its scope is the entire function, finalPrice is then changed inside the for loop, and on the last iteration it is 150 and retains that value as it exits the for loop
8) The function will return the array of discounted prices, [50, 100, 150]. Using let to declare variable does not cause issues with the functionality of the program, as the variables declared in the for loop are only needed in the for loop, and the variables declared with the entire functions scope, are needed by the entire function
9) At line 11, it will throw a ReferenceError as i is defined using let and only has scope within the for loop
10) At line 12, it will print "3" which is the length of the prices array, and this is possible because the variable is defined with const but with the entire function as its scope
11) The function will return the array of discounted prices, [50, 100, 150], this is possible even though discounted is defined as a const because the reference to the array is constant but not the data it points to, which in this case, at initialization, is an empty array
12) A. student.name;
    B. student["Grad Year"];
    C. student.greeting();
    D. student['Favorite Teacher'].name;
    E. student.courseLoad[0];
13) A. '32' , because the since '3' is a string, integer 2's string representation is '2', so the operation becomes a concatenation of strings
    B. 1 , because the subtraction operator is not defined when working with strings, so JS converts the string '3' into a number 3, becomes 3 - 2
    C. 3 , because null is the absense of any data, so you are adding 3 with 0, therefore an integer 3 is returned
    D. '3null' , because since '3' is a string and the + is used for string concatenation, null is turned into its string representation 'null'
    E. 4 , because true when being turned into an integer, is represented as 1, so the equation becomes 3 + 1 which equals 4
    F. 0 , because false when being turned into an integer is 0, and null is also represented as integer 0, so 0 + 0 = 0
    G. '3undefined' , because since '3' is a string, this equation becomes string concatenation and undefined is converted into 'undefined'
    H. NaN, because the subtraction operator is used, it converts '3' into its integer representation and then tries to convert undefined into its integer representation which it has none, which results in a NaN (Not-a-Number) and 3 - NaN = NaN
14) A. true, because '2' is converted into integer 2 because of the comparison operator, and 2 > 1 is true
    B. false, with this comparison operator on two strings, it does lexicographical comparisoins based on the first characters in the string, since '2' comes after '1' in Unicode, the comparison ends with 2 < 1 is false
    C. true, with an integer present in this comparison operater, '2' is converted into integer 2 and the comparison becomes 2 == 2 which is true
    D. false, this operator is a strict equality so it doesn't try to convert differing types, so an int is not equal to a string so returns false
    E. false, the integer representation of true is 1, so 1 == 2 returns false
    F. true, this is using strict equality, however the Boolean function returns true as long as the number given is non-zero, so Boolean(2) returns true, and the comparison becomes true === true which is true
15) The === operator is strict equality and the == operator is abstract equality. The == operator checks for equality after trying performing type coercion (changing the type of the data, '2' can be coerced into the number 2). Meanwhile the === operator does not do the type coercion, it takes everything as is, so even though '2' can be converted into 2 with ==, it will not be converted with ===. === Checks both value and type equality while == checks only == value equality.
17) The result will be [2, 4, 6] returned by the modifyArray function. The modifyArray takes in two parameters, the array you want to modify, and the reference to the function that will be modifying each individual value in the array. The for loop then loops through every value in the array that was passed in, we push a new value in newArr, that value is what is returned from the value of the passed array after being a parameter for the refenced function. In short, every value in the array that is passed in, is multiplied by 2 and stored in newArr. 
19) 1
    4
    3
    2