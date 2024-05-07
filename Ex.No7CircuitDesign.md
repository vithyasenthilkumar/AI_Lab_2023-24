# Ex.No: 7  Logic Programming –  Logic Circuit Design
### DATE: 16/03/2024                                                                           
### REGISTER NUMBER : 212221040182
### AIM: 
To write a logic program to design a circuit like half adder and half subtractor.
###  Algorithm:
1. Start the Program
2. Design a AND gate logic if both inputs are 1 then output is 1.
3. Design a OR gate logic if any one of input is 1 then output is 1.
4. Design a XOR gate logic if both inputs are different then output is 1.
5. Design a NOT gate logic if input is 0 then output is 1.
6. Design a half adder and half subtractor using the rules.
7. Test the logic.
8. Stop the program.

### Program:
```
xor(0,1,1).
xor(0,0,0).
xor(1,0,1).
xor(1,1,0).
and(1,1,1).
and(0,0,0).
and(0,1,0).
and(1,0,0).
not(0,1).
not(1,0).
or(0,1,1).
or(1,0,1).
or(0,0,0).
or(1,1,1).
halfadder(A,B,Sum,Carry):-
    xor(A,B,Sum),
    and(A,B,Carry).
halfsubtractor(A,B,Diff,Carry):-
    xor(A,B,Diff),
    not(A,C),
    and(C,B,Carry).
fulladder(A,B,Cin,S,Cout):-
    xor(A,B,X),
    xor(X,Cin,S),
    and(X,Cin,Y),
    and(A,B,Z),
    or(Y,Z,Cout).
```
### Output:
![image](https://github.com/vithyasenthilkumar/AI_Lab_2023-24/assets/127177445/4f2df2a1-eed2-4d27-a92b-00aa34ce489f)
![image](https://github.com/vithyasenthilkumar/AI_Lab_2023-24/assets/127177445/afb7121c-246a-499b-9893-5cd1e5ba881f)
![image](https://github.com/vithyasenthilkumar/AI_Lab_2023-24/assets/127177445/7b00acbb-8df6-4f87-9803-7c7f82467468)






### Result:
Thus the truth table of circuit verified sucessfully.
