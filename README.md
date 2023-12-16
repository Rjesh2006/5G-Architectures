practical 1

# Quadratic Equation Roots Calculation

import cmath

def quadratic_roots(a, b, c):
    discriminant = (b**2) - (4*a*c)
    root1 = (-b + cmath.sqrt(discriminant)) / (2*a)
    root2 = (-b - cmath.sqrt(discriminant)) / (2*a)
    return root1, root2

a = float(input("Enter coefficient a: "))
b = float(input("Enter coefficient b: "))
c = float(input("Enter coefficient c: "))

root1, root2 = quadratic_roots(a, b, c)
print(f"The roots of the equation are: {root1} and {root2}")






practica2

# Prime Number Operations

def is_prime(num):
    if num <= 1:
        return False
    for i in range(2, int(num ** 0.5) + 1):
        if num % i == 0:
            return False
    return True

def check_prime(n):
    if is_prime(n):
        print(f"{n} is a prime number.")
    else:
        print(f"{n} is not a prime number.")

# ... (Continued on next code snippet)






prac3
# Pyramid Creation


def print_pyramid(rows):
    for i in range(1, rows + 1):
        print(" " * (rows - i) + "* " * i)

def print_reverse_pyramid(rows):
    for i in range(rows, 0, -1):
        print(" " * (rows - i) + "* " * i)

num_rows = int(input("Enter the number of rows for the pyramid: "))

print("Pyramid:")
print_pyramid(num_rows)

print("\nReverse Pyramid:")
print_reverse_pyramid(num_rows)



prc 4

# Character Properties Check


def char_properties(character):
    if character.isalpha():
        if character.islower():
            print(f"The character '{character}' is a lowercase letter.")
        elif character.isupper():
            print(f"The character '{character}' is an uppercase letter.")
    elif character.isdigit():
        number_names = {...}  # Dictionary mapping numeric digits to names
        print(f"The character '{character}' is a numeric digit and its name is {number_names[character]}.")
    else:
        print(f"The character '{character}' is a special character.")

input_character = input("Enter a character: ")
char_properties(input_character)



prac5

# String Operations



def frequency_of_character(string, char):
    count = string.count(char)
    print(f"The frequency of '{char}' in the string is: {count}")

def replace_character(string, old_char, new_char):
    new_string = string.replace(old_char, new_char)
    print(f"After replacing '{old_char}' with '{new_char}': {new_string}")

# ... (Continued on next code snippet)




prc6

# Swap First 'n' Characters of Two Strings


def swap_first_n_chars(string1, string2, n):
    if n <= min(len(string1), len(string2)):
        swapped_string1 = string2[:n] + string1[n:]
        swapped_string2 = string1[:n] + string2[n:]
        return swapped_string1, swapped_string2
    else:
        return "Error: 'n' is greater than the length of one or both strings."

input_string1 = input("Enter the first string: ")
input_string2 = input("Enter the second string: ")
value_n = int(input("Enter the value of 'n': "))

result = swap_first_n_chars(input_string1, input_string2, value_n)
print(f"Swapped strings: {result[0]} and {result[1]}" if isinstance(result, tuple) else result)



prc7

# Generating Dictionary with Number Cubes

def generate_cube_dictionary():
    cube_dict = {key: key ** 3 for key in range(1, 6)}
    return cube_dict

result_dict = generate_cube_dictionary()
print("Dictionary with keys as numbers between 1 and 5 and their cubes as values:")
print(result_dict)



prc8

# Point Class and Operations


import math

class Point:
    def __init__(self, x=0, y=0):
        self.x = x
        self.y = y
    
    def __str__(self):
        return f"Point({self.x}, {self.y})"
    
    def distance(self, other_point):
        return math.sqrt((self.x - other_point.x)**2 + (self.y - other_point.y)**2)

point1 = Point(3, 4)
point2 = Point(0, 0)

print("Point 1:", point1)
print("Point 2:", point2)

distance_between_points = point1.distance(point2)
print("Distance between Point 1 and Point 2:", distance_between_points)



prc 9

# 
Dictionary Operations with Even Numbers in Tuple
def generate_cube_dictionary():
    cube_dict = {key: key ** 3 for key in range(1, 6)}
    return cube_dict

result_dict = generate_cube_dictionary()
print("Dictionary with keys as numbers between 1 and 5 and their cubes as values:")
print(result_dict)



prc 10

# Tuple Operations


t1 = (1, 2, 5, 7, 9, 2, 4, 6, 8, 10)

half_index = len(t1) // 2
print("Half the values in one line:", t1[:half_index])
print("Other half in the next line:", t1[half_index:])

even_numbers_tuple = tuple(num for num in t1 if num % 2 == 0)
print("\nTuple with even numbers:", even_numbers_tuple)

t2 = (11, 13, 15)
concatenated_tuple = t1 + t2
print("\nConcatenated tuple:", concatenated_tuple)

max_value = max(concatenated_tuple)
min_value = min(concatenated_tuple)
print("\nMaximum value:", max_value)
print("Minimum value:", min_value)




pr 11

# fliw operation and data analysis 

def count_chars_words_lines(filename):
    try:
        with open(filename, 'r') as file:
            content = file.read()
            num_chars = len(content)
            num_words = len(content.split())
            num_lines = content.count('\n') + 1  

            print(f"Total number of characters: {num_chars}")
            print(f"Total number of words: {num_words}")
            print(f"Total number of lines: {num_lines}")

            return content
    except FileNotFoundError:
        print(f"File '{filename}' not found.")

def frequency_of_characters(content):
    char_frequency = {}
    for char in content:
        if char.isalpha():
            char_frequency[char] = char_frequency.get(char, 0) + 1

    print("\nCharacter frequencies:")
    for char, frequency in char_frequency.items():
        print(f"'{char}': {frequency}")

def reverse_order_of_words(content):
    words = content.split()
    reversed_words = ' '.join(words[::-1])
    print("\nWords in reverse order:")
    print(reversed_words)

def copy_lines_to_files(filename):
    try:
        with open(filename, 'r') as file:
            lines = file.readlines()

            with open('File1.txt', 'w') as file1, open('File2.txt', 'w') as file2:
                for i, line in enumerate(lines):
                    if i % 2 == 0:
                        file1.write(line)
                    else:
                        file2.write(line)
            print("\nEven lines copied to 'File1.txt' and odd lines copied to 'File2.txt'.")
    except FileNotFoundError:
        print(f"File '{filename}' not found.")

file_name = 'sample.txt'

file_content = count_chars_words_lines(file_name)

if file_content:
    frequency_of_characters(file_content)
    reverse_order_of_words(file_content)
    copy_lines_to_files(file_name)



# user iput validation

    
prc 12

def check_name(name):
    for char in name:
        if not char.isalpha() and char != ' ':
            raise ValueError("Invalid characters in the name. Please enter a valid name.")

try:
    user_input = input("Enter your name: ")
    check_name(user_input)
    print("Name entered:", user_input)

except ValueError as e:
    print("Error:", e)
    


