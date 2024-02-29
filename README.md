# Python
Programming in Python
Write python program to print first letter of your name 
a) Example: Peter
               *      *
               *             *
               *              *
               *      *
               *
               *
               *
b) Print your name by using for loop

c) check the user name is palindrome or not
Answer:-
# Python program to print pattern G 
def Pattern(line): 
    pat="" 
    for i in range(0,line):     
        for j in range(0,line):      
            if ((j == 1 and i != 0 and i != line-1) or ((i == 0 or
                i == line-1) and j > 1 and j < line-2) or (i == ((line-1)/2) 
                and j > line-5 and j < line-1) or (j == line-2 and
                i != 0 and i != line-1 and i >=((line-1)/2))):   
                pat=pat+"*"   
            else:       
                pat=pat+" "   
        pat=pat+"\n"   
    return pat 
   

line = 7
print(Pattern(line)) 


def is_palindrome(username):
    
    username = username.lower()
    



username = input("Enter a username: ")
if is_palindrome(username):
    print(f"The username '{username}' is a palindrome!")
else:
    print(f"The username '{username}' is not a palindrome.")
