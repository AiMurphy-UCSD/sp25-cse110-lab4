1. At line 9, "values added: 20" is printed
2. At line 13, "final result: 20" is printed
3. You should not use var because it has semi-complex rules about its scope, and can lead to unnecessary issues/errors
4. At line 9, "values added: 20" is printed
5. At line 13, there is an error because changing result from var to let lost scope in the function, var reached the entire function while let only reaches the block it is contained in, therefore you are printing something that cannot be seen/is not defined
6. At line 9, there is an error, you are trying to assign a new value to a constant which is now allowed
7. At line 13, there is an error as result is not contained within the block that the print statement is trying to call from, const has the same scope as let so it will be the same error as question 5
