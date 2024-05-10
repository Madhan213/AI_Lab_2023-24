# Ex.No: 7  Logic Programming –  Logic Circuit Design
### DATE:16/03/2024                                                                            
### REGISTER NUMBER : 212221040091
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

and(0,0,0).
and(0,1,0).
and(1,0,0).
and(1,1,1).
xor(0,0,0).
xor(0,1,1).
xor(1,0,1).
xor(1,1,0).
not(0,1).
not(1,0).
halfadder(A,B,Sum,Carry):-
    xor(A,B,Sum),
    and(A,B,Carry).
halfsub(A,B,Diff,Bor):-
    xor(A,B,Diff),
    not(A,X),
    and(X,B,Bor).

```

### Output:

![Screenshot 2024-03-19 143556](https://github.com/Madhan213/AI_Lab_2023-24/assets/130206230/915a1e0c-f683-46df-ab11-41d42c7790f5)


### Result:
Thus the truth table of circuit verified sucessfully.
