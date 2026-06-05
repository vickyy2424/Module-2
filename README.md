# Built-in Functions -Binary Conversion Using Built-in Functions in Python

## 🎯 Aim
To write a Python program to convert the number **16** into its **binary representation** using built-in Python functions.

## 🧠 Algorithm
1. Assign the value `16` to a variable `a`.
2. Use the built-in `bin()` function to convert the number to binary.
3. Print the result.

## 🧾 Program:
```
a = 16
print(bin(a))
```

## Output:

<img width="1852" height="1037" alt="2a" src="https://github.com/user-attachments/assets/2de8e44e-ec33-452a-9205-192842bd4dce" />


## Result:
Thus, the program is verified successfully.
# Functions in Python: Modulo Calculator

## 🎯 Aim
To write a Python program that defines a function which accepts two values and returns their **modulo** using the `%` operator.

## 🧠 Algorithm
1. Define a function called `result` that takes two arguments `a` and `b`.
2. Inside the function, compute the modulo using `a % b`.
3. Print the result of the modulo operation.
4. Get two integer inputs from the user.
5. Call the `result` function with the user-provided values.

## 🧾 Program:
```
def result(a, b):
    print(a % b)
a = int(input())
b = int(input())
result(a, b)
```
## Output:

<img width="1857" height="1042" alt="2b" src="https://github.com/user-attachments/assets/6676f4f6-4ade-40f1-92c2-95d1abb218b1" />


## Result:
Thus, the program is verified successfully.
# Lambda Function in Python: Addition of Two Numbers

## 🎯 Aim
To write a Python program that defines a **lambda function** which takes two arguments `a` and `b`, and returns their sum.

## 🧠 Algorithm
1. Get two integer inputs from the user.
2. Use a **lambda function** to define a function `f` that returns `a + b`.
3. Call the function with the user inputs and print the result.

## 🧾 Program
```
a = int(input())
b = int(input())
f = lambda a, b: a + b
print(f(a, b))
```

## Output:

<img width="1850" height="1096" alt="2c" src="https://github.com/user-attachments/assets/ac6ed7e6-e002-47a2-8e95-51104f1d6358" />


## Result:
Thus, the program is verified successfully.
# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## 🧠 Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

---

## 🧪 Program
```
def fact(n):
    if n == 0 or n == 1:
        return 1
    else:
        return n * fact(n - 1)


rows = int(input("Enter number of rows: "))


for n in range(rows):
    print(" " * (rows - n), end="")

    for k in range(n + 1):
       
        value = fact(n) // (fact(k) * fact(n - k))
        print(value, end=" ")

    print()
```

## Sample Output

<img width="524" height="398" alt="image" src="https://github.com/user-attachments/assets/4e6b7f50-50f8-4603-8fd0-d35bb88af2ef" />


## Result
The program successfully generates Pascal’s Triangle for the given number of rows using the combination formula.
## Loops in Python: Palindrome Number Checker

## 🎯 Aim
To write a Python program that checks whether a given number is a **palindrome** using loops.

## 🧠 Algorithm
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

## 🧾 Program
```
num=int(input()) 

rev=0 

temp=num 

while temp>0: 

    rev=(10*rev)+temp%10 

    temp//=10 

    if rev==num: 

        print("The given number {} is a Palindrome".format(num)) 

    else: 

        print("The given number {} is not a palindrome".format(num))
```
## Output

<img width="593" height="114" alt="image" src="https://github.com/user-attachments/assets/fbc45cbf-8cf2-47de-947f-58a2e7d476f2" />

## Result

Thus, the program has been successfully executed .
