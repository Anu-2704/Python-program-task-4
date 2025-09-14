# Python-program-task-4
import random
import string

# Step 1: Take user input for password length
length = int(input("Enter the desired password length: "))

# Step 2: Define possible characters for the password
characters = string.ascii_letters + string.digits + string.punctuation
# ascii_letters = a-z, A-Z
# digits = 0-9
# punctuation = special characters !@#$%^&*()

# Step 3: Generate password
password = ''.join(random.choice(characters) for i in range(length))

# Step 4: Display the password
print("Your generated password is:", password)
