                                     Assignment #1
Student:Tumenbai Aidana
Group: SE-2511

Task 1 
![photo_5325760551306597793_w](https://github.com/user-attachments/assets/a55ab9b8-2ef8-4f30-b650-c64583bde6b9)
If the number is a single digit (n < 10), print it.
First call the function recursively with n / 10 (the number without the last digit), then print n % 10 (the last digit).
This order ensures that digits are printed from left to right. For example, with input 5481:
1. Call printDigits(548) → then print 1
2. Call printDigits(54) → then print 8
3. Call printDigits(5) → print 5
4. Output: 5, 4, 8, 1
 
Task 2
![photo_5325760551306597923_w](https://github.com/user-attachments/assets/a75fd535-24e7-48d6-b5ac-fc5ee8605f91)
Create a recursive function to calculate the sum of array elements. The function takes an array and an index to start from.
If the index equals the array length (reached the end), return 0.
Return arr[index] + sum(arr, index + 1).
After obtaining the sum, calculate the average using the formula:
average = sum / array.length (where array.length is the total number of elements).
Example for array [3, 2, 4, 1]:
1. sum([3,2,4,1], 0) = 3 + sum([3,2,4,1], 1)
2. sum([3,2,4,1], 1) = 2 + sum([3,2,4,1], 2)
3. sum([3,2,4,1], 2) = 4 + sum([3,2,4,1], 3)
4. sum([3,2,4,1], 3) = 1 + sum([3,2,4,1], 4)
5. sum([3,2,4,1], 4) = 0
Sum calculation: 3 + 2 + 4 + 1 + 0 = 10
Average:10/4=2.5
Output: 2.5

Task 3
![photo_5325760551306597923_w](https://github.com/user-attachments/assets/ecc27e91-9233-41cb-92fd-451296194817)
The function starts checking divisors from 2.
If the number is 1 or less  it’s not prime.
If the divisor squared is greater than the number it’s prime (no divisors found).
If the number is divisible by the divisor  it’s not prime.
Call the function again with the next divisor (divisor + 1).
Number = 7  Prime
Number = 10 Not Prime

Task 4
![photo_5325760551306597947_w](https://github.com/user-attachments/assets/c4134543-f521-4c7f-b665-7d2aeb68ce4c)
If n == 0  return 1 (because 0! = 1).
Return n * factorial(n - 1).
factorial(5) = 5 × factorial(4)
factorial(4) = 4 × factorial(3)
factorial(3) = 3 × factorial(2)
factorial(2) = 2 × factorial(1)
factorial(1) = 1 × factorial(0)
factorial(0) = 1
Multiply everything: 5 × 4 × 3 × 2 × 1 = 120

Task 5
![photo_5325760551306597960_w](https://github.com/user-attachments/assets/b2c1dec0-7e5c-45f4-bcfa-d9d84d96384f)
Formula:𝐹𝑛 = 𝐹𝑛−1 + 𝐹𝑛−2 
Base cases : 𝐹0 =0,𝐹1 =1

Task 6
![photo_5325760551306597971_y](https://github.com/user-attachments/assets/60b60f7a-de84-4a54-a9bf-17d6374adc18)
Base case:If n == 0 return 1 (because any number to the 0th power is 1)
Recursive case:Return a * power(a, n - 1)

Task 7

Task 8
![photo_5325760551306598069_y](https://github.com/user-attachments/assets/6007fe0a-f0ea-4c67-9223-9752e85223a3)
First, as the base case, I returned "Yes" if the string was empty, because all characters had been checked.
In the recursive case, I checked if the first character was a digit:
If it wasn’t a digit, I returned "No".
If it was a digit, I called the function on the rest of the string and continued checking recursively

Task 9
![photo_5325760551306598075_y](https://github.com/user-attachments/assets/6ea59ee6-0fa1-4e98-a2a9-30a3baedd0bc)
Write a recursive function that counts the number of characters in a given string. The function should return the total number of characters in the string.
Base Case: If the string is empty (""), its length is 0.
Recursive Case: The length of a string is 1 (for the first character) plus the length of the rest of the string (the substring starting from the second character).
The function calls itself recursively with the string minus its first character, adding 1 each time, until the string becomes empty.
Example for "hello":
countChars("hello")  1 + countChars("ello")
countChars("ello")  1 + countChars("llo")
countChars("llo")  1 + countChars("lo")
countChars("lo")  1 + countChars("o")
countChars("o")  1 + countChars("")
countChars("")  0 (Base case)
Results: 1 + 1 + 1 + 1 + 1 + 0 = 5
Output: 5

Task 10
![photo_5325760551306598083_w](https://github.com/user-attachments/assets/0dbe144d-d5d1-4b7c-85e9-31e8397ec6ab)
Write a recursive function that finds the GCD of two numbers using the Euclidean Algorithm.
If the second number b is 0, then the GCD is a (since GCD(a, 0) = a).
According to the Euclidean Algorithm, GCD(a, b) = GCD(b, a % b). The function calls itself with b as the new first number and a % b as the new second number, repeating until the second number becomes 0.
Example for 32 and 48:
gcd(32, 48) gcd(48, 32 % 48) → gcd(48, 32)
gcd(48, 32)  gcd(32, 48 % 32) → gcd(32, 16)
gcd(32, 16)  gcd(16, 32 % 16) → gcd(16, 0)
gcd(16, 0)  16 (Base case)
Output: 16
