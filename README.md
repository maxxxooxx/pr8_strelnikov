# Лабораторная работа N8
import random
import string

def generate_password(length=11):
"""Generate a random password of given length (default 11)"""
# define possible characters
chars = string.ascii_letters + string.digits + string.punctuation

# generate password
password = ''.join(random.choice(chars) for i in range(length))

return password

# example usage
password = generate_password()
print(password)
