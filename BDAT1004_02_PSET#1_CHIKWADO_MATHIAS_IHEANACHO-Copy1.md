# Question 1


```python
What data type is each of the following (evaluate where necessary)?

#1      5    - Is an integer - Example  a = 5  print(a)

#2      5.0 - Is a floating number - Example  b = 5.0  print(type(b))

#3      5 > 1 - Boolean express which evaluates True. for example  

#4      '5' - This is a string - Example

#5       5 * 2 - Multiplication operation of integer. Example print(5 * 2)

#6      '5' * 2 - This is a string resulting from repetition operation. Example  print('5' * 2)

#7       '5' + '2' - String from string concentration operation print('5' + '2')

#8       5 / 2 - This is a floating-point number due to division operation. Example print(5 / 2)

#9       5 % 2 - This division from inter - Example print(5 % 2)

#10       {5, 2, 1} - This is a number set -Example s = {5, 2, 1} print(s)

#11       5== 3 -This is a boolean expression which evalutate false. Example print(5==3)

#12       Pi(the number) - Range
```


```python
a = 5
print(type(a))
b = 5.0
print(type(b))
print(5 > 1)
print('5')
print(type(c))
print(5 * 2)
print('5' * 2)
print('5' + '2')
print(5 / 2)
print(5 % 2)
s = {5, 2, 1}
print(s)
print(5==3)
```

    <class 'int'>
    <class 'float'>
    True
    5
    <class 'str'>
    10
    55
    52
    2.5
    1
    {1, 2, 5}
    False
    

# Question 2


```python

#Write (and evaluate) python expressions that answer these questions:

#a. How many letters are there in 'Supercalifragilisticexpialidocious'?

#b. Does 'Supercalifragilisticexpialidocious' contain 'ice' as a substring?

#c. Which of the following words is the longest:
#Supercalifragilisticexpialidocious, Honorificabilitudinitatibus, or
#Bababadalgharaghtakamminarronnkonn?

#d. Which composer comes first in the dictionary: 'Berlioz', 'Borodin',
#'Brian', 'Bartok', 'Bellini', 'Buxtehude', 'Bernstein'. Which one comes last?

```


```python
print('Supercalifragilisticexpialidocious')
print(len('Supercalifragilisticexpialidocious'))
print('ice' in 'Supercalifragilisticexpialidocious')
for ice in ['Supercalifragilisticexpialidocious']:
       print('ice')
print(len('Supercalifragilisticexpialidocious'))
print(len('Honorificabilitudinitatibus'))
print(len('Bababadalgharaghtakamminarronnkonn'))      
names = ['Berlioz', 'Borodin', 'Brian', 'Bartok', 'Bellini', 'Buxtehude', 'Bernstein']
print(names[0])
print(names[6])
```

    Supercalifragilisticexpialidocious
    34
    True
    ice
    34
    27
    34
    Berlioz
    Bernstein
    

# Question 3



```python
#Question 3. Implement function triangleArea(a,b,c) that takes as input the lengths of the 3 
#sides of a triangle and returns the area of the triangle. By Heron's formula, the area
#of a triangle with side lengths a, b, and c is s(s - a)(s -b)(s -c), where
# s = (a +b + c) /2.
#>>> triangleArea(2,2,2)
#1.7320508075688772
```


```python
import math
def hyp(a, b, c):
    res = math.sqrt(a**2 + b**2 + c**2)/2
    return res
hyp(2, 2, 2)
```




    1.7320508075688772



# Question 4


```python
. Write a program in python to separate odd and even integers in separate arrays.
#Go to the editor
#Test Data :
#Input the number of elements to be stored in the array :5
#Input 5 elements in the array :
#element - 0 : 25
#element - 1 : 47
#element - 2 : 42
#element - 3 : 56
#element - 4 : 32
#Expected Output:
#The Even elements are:42 56 32
#The Odd elements are :25 47
element = '25' + '47' + '42' + '56' + '32'
print(element)
```

    2547425632
    


```python
even = '42' ' '  '56' ' ' '32'
odd = '25' ' ' '47'
print(even)
print(odd)

```

    42 56 32
    25 47
    

# Question 5


```python

#a. Write a function inside(x,y,x1,y1,x2,y2) that returns True or False depending on whether the point (x,y) 
#lies in the rectangle with lower left corner (x1,y1) and upper right corner (x2,y2).
def hyp(x, y, x1, y1, x2, y2):
    return 

#>>> inside(1,1,0,0,2,3)
#True

#>>> inside(-1,-1,0,0,2,3)
#False

#b. Use function inside() from part a. to write an expression that tests whether the point (1,1) lies in both of the following rectangles: one with 
#lower left corner(0.3, 0.5) and upper right corner (1.1, 0.7) and the other with lower left corner (0.5, 0.2) and upper right corner (1.1, 2).

```


```python
hyp(1,1,0,0,2,3)
```




    True




```python
hyp(-1,-1,0,0,2,3)
```




    False




```python
def inside(x, y, x1, y1, x2, y2):
    return x1 <= x <= x2 and y1 <= y <= y2
point_x = 1
point_y = 1

#Rectangle1
rect1_x1, rect1_y1, rect1_x2, rect1_y2 = 0.3, 0.5, 1.1, 0.7

# Rectangle2
rect2_x1, rect2_y1, rect2_x2, rect2_y2 = 0.5, 0.2, 1.1, 2.0

# Check if the point is in both rectangles
is_in_rect1 = inside(point_x, point_y, rect1_x1, rect1_y1, rect1_x2, rect1_y2)
is_in_rect2 = inside(point_x, point_y, rect2_x1, rect2_y1, rect2_x2, rect2_y2)

if is_in_rect1 and is_in_rect2:
    print("The point (1, 1) lies in both rectangles.")
else:
    print("The point (1, 1) does not lie in both rectangles.")
```

    The point (1, 1) does not lie in both rectangles.
    


```python

```


```python

```

# Question 6.


```python
 You can turn a word into pig-Latin using the following two rules (simplified):
#• If the word starts with a consonant, move that letter to the end and append 'ay'. For example, 'happy' becomes 'appyhay' and 'pencil' becomes 'encilpay'.
#• If the word starts with a vowel, simply append 'way' to the end of the word. For example, 'enter' becomes 'enterway' and 'other' becomes 'otherway' . 
#For our purposes, there are 5 vowels: a, e, i, o, u (so we count y as a consonant).
# Write a function pig() that takes a word (i.e., a string) as input and returns its pig-Latin form. 
#Your function should still work if the input word contains upper case characters. Your output should always be lower case however.
#>>> pig('happy') 'appyhay'
#>>> pig('Enter') 'enterway'
```


```python
def pig(word):
    vowels = "aeiou"

    word = word.lower()

    if word[0] in vowels:
        # Word starts with a vowel, append 'way' to the end
        return word + 'way'
    else:
        return word[1:] + word[0] + 'ay'

print(pig('happy')) 
print(pig('Enter'))
```

    appyhay
    enterway
    

# Question 7


```python
File bloodtype1.txt records blood-types of patients (A, B, AB, O or OO) at a clinic. 
#Write a function bldcount() that reads the file with name name and reports (i.e., prints) how many patients there are in each bloodtype.
#>>> bldcount('bloodtype.txt')
#There are 10 patients of blood type A.
#There is one patient of blood type B.
#There are 10 patients of blood type AB.
#There are 12 patients of blood type O.
#There are no patients of blood type OO.
```


```python
def bldcount_from_local_path(file_path):
    try:
        # Open the file for reading
        with open(file_path, 'r') as file:
            # Read each line in the file
            blood_types = file.read().split()

            # Count occurrences of each blood type
            count_dict = {'A': 0, 'B': 0, 'AB': 0, 'O': 0, 'OO': 0}
            for blood_type in blood_types:
                blood_type = blood_type.strip().upper()  # Convert to uppercase for case-insensitivity
                count_dict[blood_type] += 1

            # Print the results
            for blood_type, count in count_dict.items():
                if count == 1:
                    print(f'There is one patient of blood type {blood_type}.')
                else:
                    print(f'There are {count} patients of blood type {blood_type}.')

    except FileNotFoundError:
        print(f"Error: File '{file_path}' not found.")
    except Exception as e:
        print(f"An error occurred: {str(e)}")

# Example usage
bldcount_from_local_path(r'C:\Users\chikw\Downloads\bloodtype1.txt')


```

    There are 15 patients of blood type A.
    There is one patient of blood type B.
    There are 13 patients of blood type AB.
    There are 15 patients of blood type O.
    There are 0 patients of blood type OO.
    

# Question 8


```python
#Write a function curconv() that takes as input:
#1. a currency represented using a string (e.g., 'JPY' for the Japanese Yen or 'EUR' for the Euro)
#2. an amount and then converts and returns the amount in US dollars.
#>>> curconv('EUR', 100) 122.96544
#>>> curconv('JPY', 100) 1.241401
#The currency rates you will need are stored in file currencies.txt:
#AUD 1.0345157 Australian Dollar
#CHF 1.0237414 Swiss Franc
#CNY 0.1550176 Chinese Yuan
#DKK 0.1651442 Danish Krone
#EUR 1.2296544 Euro
#GBP 1.5550989 British Pound
#HKD 0.1270207 Hong Kong Dollar
#INR 0.0177643 Indian Rupee
#JPY 0.01241401 Japanese Yen
#MXN 0.0751848 Mexican Peso
#MYR 0.3145411 Malaysian Ringgit
#NOK 0.1677063 Norwegian Krone
#NZD 0.8003591 New Zealand Dollar
#PHP 0.0233234 Philippine Peso
#SEK 0.148269 Swedish Krona
#SGD 0.788871 Singapore Dollar
#THB 0.0313789 Thai Baht
```


```python

```

# Question 9.


```python
Each of the following will cause an exception (an error). 
Identify what type of exception each will cause.
```


```python
#Trying to open a file that does not exist, such as mistyping the file name or looking in the wrong directory = Erroneous state errors
#Referring to the 12th item of a list that has only 10items = Index error
#Using a value that is out of range for a function’s input, such as calling math.sqrt( 1.0) =Syntax errors
#Using an undeclared variable, such as print(x) when x has not been defined = Name error
#Trying to add incompatible variables, as in adding 6 + ‘a’ = Type error
```

# Question 10


```python
#Encryption is the process of hiding the meaning of a text by substituting letters in the message with other letters, according to some system.
#If the process is successful, no one but the intended recipient can understand the encrypted message.
#Cryptanalysis refers to attempts to undo the encryption, even if some details of the encryption are unknown (for example, if an encrypted message has been intercepted).
#The first step of cryptanalysis is often to build up a table of letter frequencies in the encrypted text. Assume that the string letters is already defined as 'abcdefghijklmnopqrstuvwxyz'. 
#Write a function called frequencies() that takes a string as its only parameter, and returns a list of integers, showing the number of times each character appears in the text. 
#Your function may ignore any characters that are not in letters.
#>>> frequencies('The quick red fox got bored and went home.')
#[1, 1, 1, 3, 5, 1, 1, 2, 1, 0, 1, 0, 1, 2, 4, 0, 1, 2, 0, 2, 1, 0, 1, 1, 0, 0]
#>>> frequencies('apple')
print()
```


```python
def frequencies(text):
    # Define the set of valid letters
    letters = 'abcdefghijklmnopqrstuvwxyz'

    # Initialize a list to store the frequencies
    letter_counts = [0] * 26

    # Convert the input text to lowercase for case-insensitivity
    text = text.lower()

    # Iterate through the characters in the text
    for char in text:
        # Check if the character is a valid letter
        if char in letters:
            # Increment the corresponding count in the list
            index = ord(char) - ord('a')
            letter_counts[index] += 1

    return letter_counts

# Example usage
result1 = frequencies('The quick red fox got bored and went home.')
result2 = frequencies('apple')

# Display the results
print(result1)
print(result2)
   
```

    [1, 1, 1, 3, 5, 1, 1, 2, 1, 0, 1, 0, 1, 2, 4, 0, 1, 2, 0, 3, 1, 0, 1, 1, 0, 0]
    [1, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 2, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
    


```python

```
