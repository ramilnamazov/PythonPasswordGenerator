import random  # Importing the random module to use its functions
import string  # Importing the string module to get a set of characters

def generate_password(length: int = 10):  # Define a function to generate a password, with a default length of 10 characters
    alphabet = string.ascii_letters + string.digits + string.punctuation  # Create a string of all letters (uppercase and lowercase), digits, and punctuation
    password = ''.join(random.choice(alphabet) for i in range(length))  # Randomly choose 'length' number of characters from 'alphabet' and join them into a string
    return password  # Return the generated password

password = generate_password()  # Call the function to generate a password and store it in the variable 'password'
print(f"Generated Password: {password}")  # Print the generated password
