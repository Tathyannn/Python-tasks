# Check if a number is even or odd

num = int(input("Enter a number: "))

if num % 2 == 0:
    print(f"{num} is Even")
else:
    print(f"{num} is Odd")



# Calculate factorial of a number

n = int(input("Enter n: "))
factorial = 1

for i in range(1, n + 1):
    factorial *= i

print(f"Factorial of {n} is: {factorial}")



# Find the maximum number in a list

numbers = [12, 45, 2, 89, 34, 67]

# Version 1
max_val = max(numbers)

# Version 2
# max_val = numbers[0]
# for num in numbers:
#     if num > max_val:
#         max_val = num

print(f"Maximum value is: {max_val}")



# Reverse a string

text = input("Enter a word: ")
reversed_text = text[::-1]

print(f"Reversed: {reversed_text}")



# Check if a word is a palindrome

word = input("Enter a word: ").lower()

if word == word[::-1]:
    print(f"'{word}' is a palindrome!")
else:
    print(f"'{word}' is NOT a palindrome.")



# Check if a number is a prime number

num = int(input("Enter a number: "))

if num > 1:
    is_prime = True
    for i in range(2, int(num ** 0.5) + 1):
        if num % i == 0:
            is_prime = False
            break

    if is_prime:
        print(f"{num} is a Prime number")
    else:
        print(f"{num} is NOT a Prime number")
else:
    print(f"{num} is NOT a Prime number")



# Calculate the average of numbers in a list

numbers = [10, 20, 30, 40, 50]

total_sum = sum(numbers)
count = len(numbers)

average = total_sum / count

print(f"The average is: {average}")
