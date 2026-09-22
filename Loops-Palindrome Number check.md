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
num = int(input("Enter a number: "))
original = num
reversed_num = 0
while num > 0:
    digit = num % 10
    reversed_num = reversed_num * 10 + digit
    num = num // 10
if original == reversed_num:
    print("The number is a palindrome.")
else:
    print("The number is not a palindrome.")
```
## Output
<img width="1041" height="364" alt="502893398-263005ac-a9ad-4859-be77-a4cce641c52f" src="https://github.com/user-attachments/assets/2846d201-c7be-4766-b9d9-cfa90f99ad1f" />


## Result
The Python program that checks whether a given number is a palindrome using loops is executed successfully.
