# 19CS301-Module7
# EX: 7.1 RECURSION
### Aim: 
To write a Python program that counts the number of 1's in a binary number using a recursive function.
### Algorithm:
1.	Start the program.
2.	Define a recursive function count_ones(binary_str) that accepts a binary string as input.
3.	In the function, check if the string is empty:
-	If it is, return 0 (base case).
4.	Otherwise:
-	If the first character is '1', return 1 plus the recursive call on the rest of the string.
-	Else, return 0 plus the recursive call on the rest of the string.
5.	Read the binary string input from the user.
6.	Call the recursive function and print the result.
7.	End the program.


### Program:
```
#Reg.NO:212222040120
#Name:PRASANNA R
def count_ones(binary_str):
    # Base case: if the string is empty, return 0
    if not binary_str:
        return 0
    # Recursive case: check the first character and add to the count if it's '1'
    return (1 if binary_str[0] == '1' else 0) + count_ones(binary_str[1:])

# Example usage
binary_input = input()
result = count_ones(binary_input)
print(result)

```
### Output:
![image](https://github.com/user-attachments/assets/39537092-31b9-484d-8a57-1c1d4045fbdb)


### Result:
Thus, the given program is implemented and executed successfully .
 

# EX: 7.2 TYPES OF RECURSIONS
### Aim: 
To write a Python program that displays the first n Fibonacci numbers using tree recursion.
### Algorithm:
1.	Start the program.
2.	Define a recursive function fibonacci(n):
       -	If n == 0, return 0.
       -	If n == 1, return 1.
       -	Else, return fibonacci(n-1) + fibonacci(n-2).
3.	Read an integer n_terms from the user.
4.	If n_terms <= 0, print an error message.
5.	Else, iterate from 0 to n_terms - 1 and print the Fibonacci number using the fibonacci(i) function.
6.	End the program.

### Program:
```
#Reg.NO:212222040120
#Name:PRASANNA R
def fibonacci(n):
    if n==0:
        return 0
    if n==1:
        return 1
    else:
        return fibonacci(n-1)+fibonacci(n-2)

```
### Output:
![image](https://github.com/user-attachments/assets/9f528371-3382-4d19-95e8-2cddd6eee7e6)

### Result: 
Thus, the given program is implemented and executed successfully .


# EX: 7.3 TAYLOR SERIES

### Aim: 
To Write a python program to evaluate the series using recursion.
### ALGORITHM:
1.	Start the program.
2.	Define a recursive function evaluate_series(x, n):
       o	If n == 0, return 1.
       o	Else, return 3**n * x**n + evaluate_series(x, n-1).
3.	Take input values for x and n from the user.
4.	Call the recursive function and print the result.
5.	End the program.


### Program:
```
#Reg.NO:212222040120
#Name:PRASANNA R
def series(x,n):
    if n<=0:
        return 1
    else:
        return ((3**n)*(x**n))+series(x,n-1)
x=int(input())
n=int(input())
print(series(x,n))
```
### Output:
![image](https://github.com/user-attachments/assets/4423b074-3e24-4b8a-b15f-d091075c3a0f)

 
### Result: 
Thus, the given program is implemented and executed successfully .
 

# EX: 7.4 Solve by recursion relation

### Aim: 
To write a Python program to determine the sum of all elements in a list using recursion.

### Algorithm:
1.	Start the program.
2.	Define a recursive function sum_list(lst, n):
       -	If n == 0, return lst[0].
       -	Else, return lst[n] + sum_list(lst, n - 1).
3.	Get the number of elements in the list from the user.
4.	Input each element and store in a list.
5.	Call the recursive function with the list and its last index.
6.	Print the result.
7.	End the program.



### Program:
```
#Reg.NO:212222040120
#Name:PRASANNA R
def sum_list(l,length):
    if length==0:
        return l[0]
    else:
        return l[length]+sum_list(l,length-1)
    
l=[]
n=int(input())
for i in range(n):
    x=int(input())
    l.append(x)

```
### Output:
![image](https://github.com/user-attachments/assets/bb830779-ab23-491b-a75f-84cf664342fa)

### Result: 
Thus, the given program is implemented and executed successfully .
 

