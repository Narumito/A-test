#Below are some examples done in a class where we practice Python + some of my tests using Loops

#Centered title
txt = "Welcome to trial number 2!"
z = txt.center(80)
print(z)
from turtle import position


print()

#Week 1 practices
print("A. This is Week 1 practice in class".center(40))
print()

#Using Operators
print("Ex1:")
x=5
y=10
print("x + y = ")
print(x+y)
print("x - y = ")
print(x-y)
print("x / y = ")
print(x/y)
print("x * y = ")
print(x*y)

print()

#Using Nested If statement
print("Ex2:")
x = int (input("Insert a value for x"))
y = int (input("Insert a value for y"))

if x>0 and y>0:
    if x>y:
        print("x greater than y")
    elif x<y:
        print("x lesser than y")
    elif x==y:
        print("x is equal to y")
    else:
        print("x and y are invalid")
else:
    print ("Please add a valid positive number for x and y!")

print()'''

#Week 2 exercises
    
'''#Ex1: Using Operators
a = int(input("Choose a value for a: "))
b = int(input("Choose a value for b: "))
print("Now we will process some opertations such as:")
# addition
print ('Addition: ', a + b)  

# subtraction
print ('Subtraction: ', a - b)   

# multiplication
print ('Multiplication: ', a * b)  

# division
print ('Division: ', a / b) 

# floor division
print ('Floor Division: ', a // b)

# modulo
print ('Modulo: ', a % b)  

# a to the power b
print ('Power: ', a ** b) '''

print()

'''#Ex2: Using Assignment Operators
print("For the second example we will create operations using Assignment Operators:")
#Assigning 5 to r
r=5
print("= : r=" + str(r))

#Addition Assignment
r += 1
print("+= : r += 1 => " + str(r))

#Subtraction Assignment
r -= 3
print("-= : r -= 3 => " + str(r))

#Multiplication Assignment
r *= 4
print("*= : r *= 4 => " + str(r))

#Division Assignment
r /= 3
print("/= : r /= 3 => " + str(r))

#Remainder Assignment
r %= 10
print("%= : r %= 10 => " + str(r))

#Exponent Assignment
r **= 10 
print("**= : r **= 10 => " + str(r)) '''

print()

'''Extra
# assign 10 to t
t = 10

# assign 5 to s
s = 5 

# assign the sum of a and b to a
t += s      # t = t + s

print(t)

# Output: 15'''

print()

'''#Comparison Operators
d = int(input("Choose a value for d: "))

e = int(input("Choose a value for e: "))

# equal to operator
print('d == e =', d == e)

# not equal to operator
print('d != e =', d != e)

# greater than operator
print('d > e =', d > e)

# less than operator
print('d < e =', d < e)

# greater than or equal to operator
print('d >= e =', d >= e)

# less than or equal to operator
print('d <= e =', d <= e) '''


'''#Experimental use of a Loop
print("B. This is a test for a loop program".center(47))
print()

while True:
    randomnr = int( input ("Enter a random number:"))
    try:
        if randomnr < 5:
            print ("MIAW POW")
        else:
            print (f"NOT MIAW POW! If you are not pleased insert another number:")
    except ValueError:
        print ("If not pleased try another number!!")
        

    cont = input ("Want to try another nr? (y/n)")
    if cont != "y":
        break   
 '''
 
 #Data Structure
 #Lists
#A list of strings focusing on Fluffy animals
'''
fluffy_animals = ['Pallas_Cat', 'Red Panda', 'Arctic Fox', 'English Angora Rabbit',
'Pomeranian', 'Alpaca', 'Snow Leopard', 'Chinchilla', 'Black and White Ruffed Lemur', 'Baby Duck']

print(fluffy_animals)
print(fluffy_animals [5])

fluffy_animals.append('Squirel')
print(fluffy_animals)
'''
#Another list of strings focusing on Mountains
'''tall_mountains = ['Everest', 'K2', 'Yr Wyddfa']
print(tall_mountains)
#Adding more values to Mountains list
mountains = tall_mountains
mountains.extend(['Ben Nevis', 'Mauna', 'Margherita'])

for mountain in mountains:
    print(mountain)
    '''
#List of random numbers
'''r_numbers = [33, 66, 313, 3213, 43, 63, 99]
user_number = int(input('Type any number: '))

if user_number in r_numbers:
    print("%d is in the Special Hidden List!" % user_number)
    
if user_number not in r_numbers:
    print("%d is not in the Special Hidden List!" % user_number)'''
    
#Ex3 - creating 2 sets of numbers a(first 4 integers) and b(first odd integers)
'''a = {1, 2, 3, 4}
b = {1, 3, 5, 7}
#combining the numbers from a or b or both
c = a|b 
#containing the numbers in a but not on b
d = a-b 
#containing the numbers in b but not on a
e = b-a 
#containing the numbers from both a and b
f = a & b 
#containing the number from either a or b but not both
g = a ^ b 

print(len(c)) 
print(c, d, e, f, g)'''

#dictionaries example + modify the value of red
'''marble = {"red": 34}
marble["red"] += 3
print(marble["red"])'''

#Testing disctionaries
'''#Defining some coordinates to be guesed
battle = {
(3, 4): False,
(2, 6): True
}

#loop command for user input and answers
def Battle_Position (battle):
    while True:
        try:
            x = int(input("Enter the first value for a coordinate x:"))
            y = int(input("Enter the second value for a coordinate y:"))
            position = (x, y)
        except ValueError:
            print("Invalid value")
            continue
        
        if position in battle:
            if battle[position]:
                print(f'position {position} is True')
                break
            else:
                print(f'position {position} is False') 
        else:
            print(f'position {position} NA')
Battle_Position(battle)'''
