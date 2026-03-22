                                     Assignment #1
Student:Tumenbai Aidana
Group: SE-2511

Task 1 
![photo_5325760551306597793_w](https://github.com/user-attachments/assets/a55ab9b8-2ef8-4f30-b650-c64583bde6b9)
It keeps dividing the number by 10 until only one digit remains, thus reducing a large number to a smaller one. If the number is 0, it stops. n % 10 takes the last digit.
Task 2![photo_5330108673117852841_y](https://github.com/user-attachments/assets/feec8cb5-3096-407a-8de7-a1e68327c194)
When n == 0, meaning all elements have been added, the function returns the average. If n is greater than 0, the function keeps calling itself, and each time it is called, it adds the last element
Task 3
![photo_5325760551306597923_w](https://github.com/user-attachments/assets/ecc27e91-9233-41cb-92fd-451296194817)
If the number is less than or equal to 2:
2 is a prime number, so true is returned
0 or 1 is not a prime number, so false is returned
If the number n is divisible by i, then n is not a prime number, so false is returned
If the square of the divisor is greater than n, then n is considered a prime number, because we have checked all possible divisors, so true is returned
If none of the above conditions are met, the function calls itself again

Task 4
![photo_5325760551306597947_w](https://github.com/user-attachments/assets/c4134543-f521-4c7f-b665-7d2aeb68ce4c)
If n is 1, the factorial is equal to 1, so it returns 1. If n is greater than 1, the function calls itself and multiplies it by n 
part 2
Task 5
![photo_5325760551306597960_w](https://github.com/user-attachments/assets/b2c1dec0-7e5c-45f4-bcfa-d9d84d96384f)
If n > 1, the function calls itself twice:
fib(n-1) the previous Fibonacci number
fib(n-2) the Fibonacci number before that It adds these two numbers to calculate the Fibonacci number

Task 6
![photo_5325760551306597971_y](https://github.com/user-attachments/assets/60b60f7a-de84-4a54-a9bf-17d6374adc18)
Any number raised to the power of 0 equals 1, so if n = 0, it returns 1. If n > 0, the function calls itself and then multiplies the result by a

Task 7

Task 8
![photo_5325760551306598069_y](https://github.com/user-attachments/assets/6007fe0a-f0ea-4c67-9223-9752e85223a3)
If i reaches the end of the string, meaning all characters have been checked, then the string is considered to consist only of digits, so it returns true. If the current character (s.charAt(i)) is not a digit, then the string contains a non-digit character, so it returns false. If the current character is a digit, the function calls itself for the next character (i+1)

Task 9
![photo_5325760551306598075_y](https://github.com/user-attachments/assets/6ea59ee6-0fa1-4e98-a2a9-30a3baedd0bc)
If the string is empty (""), its length is 0, so it returns 0. If the string is not empty, the function calls itself, but removes the first character of the string (s.substring(1)). Each recursive call adds 1

Task 10
![photo_5325760551306598083_w](https://github.com/user-attachments/assets/0dbe144d-d5d1-4b7c-85e9-31e8397ec6ab)
If the second number b is 0, the GCD equals the first number, because when dividing by 0 there is no remainder. Therefore, it returns a. If b is not 0, the function calls itself with new parameters:
·first parameter = the second number b
second parameter = the remainder when a is divided by b (a % b)
 This works according to the Euclidean algorithm
