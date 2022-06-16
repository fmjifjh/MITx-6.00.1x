# MITx-6.00.1x
Introduction to Computer Science and Programming Using Python


# Unit 1: Python basics / 2. Core elements of programs / Exercise: While

# 1) While

x = 2
while x <= 10:   
    print(x)
    x += 2
print("Goodbye!")

# 2) While

print("Hello!")
y = 10
while y >= 2:     
     print(y)
     y -= 2
     
# 3) While

final = 0
now = 1
while now <= final:
    final += now 
    now += 1
print(final)


# 1) For




# PROBLEM SET 1
# Exercise 1
vowels = 0

for char in s:
    if char == 'a' or char == 'e' or char == 'i' \
       or char == 'o' or char == 'u':
        vowels += 1
print("Number of vowels:" + " " +str(vowels))

# Exercise 2

bob = 0

for i in range(len(s)):
    if s[i:i+3] == "bob":
        bob += 1
print("Number of times bob occurs is:" + " " +str(bob))


# Exercise 3

s = 'ywlxuynnkalyoyoohmz'
string_A = s[0]
string_C = ""
string_N = ""

for i in range(1,len(s)):
           
    if s[i] >= s[i-1]:                    
        string_A += s[i]
                
    if s[i] < s[i-1]:
        
        string_C = string_A
        if len(string_C) > len(string_N):
            
            string_N = string_C
            
        elif len(string_C)==len(string_N):
            string_C = string_N
            
        string_A = ""
        string_A += s[i]
                             
if len(string_A) > len(string_N):

    string_N = string_A

elif len(string_A) == len(string_N):
    string_A = string_N
else:
    string_A = string_N    
                       
print("Longest substring in alphabetical order is:" + " " +str(string_A))

