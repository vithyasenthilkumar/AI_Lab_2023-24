# Ex.No: 5   Logic Programming – Factorial of number   
### DATE: 09/03/2024                                                                            
### REGISTER NUMBER : 212221040182 
### AIM: 
To  write  a logic program for finding the factorial of given number using SWI-PROLOG. 
### Algorithm:
1. STEP 1: Start the program
2. STEP 2:  Write a rules for finding factorial of given program in SWI-PROLOG.
3.   a)	factorial of 0 is 1 => written as factorial(0,1).
4.   b)	factorial of number greater than 0 obtained by recursively calling the factorial    function.
5. STEP 3: Run the program  to find answer of  query.
6. STEP 4: Stop the program.

### Program:
```
factorial(0,1).
factorial(A,B) :-  
           A > 0, 
           C is A-1,
           factorial(C,D),
           B is A*D.
```



### Output:
![Factorial Result](https://github.com/vithyasenthilkumar/AI_Lab_2023-24/assets/127177445/f614ffd9-ff04-4128-a03c-d2f53053b5e1)





### Result:
Thus the factorial of given number was found by logic programming. 
