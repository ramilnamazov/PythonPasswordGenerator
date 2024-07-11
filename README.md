# Python Password Generator

## Overview

This project is a simple password generator script written in Python. It generates a random password containing letters, digits, and punctuation characters. The default password length is 10 characters, but it can be customized.

## Features

- Generates a random password
- Uses a mix of uppercase letters, lowercase letters, digits, and punctuation characters
- Default password length is 10 characters, but can be modified

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/ramilnamazov/PythonPasswordGenerator.git
    ```

2. Navigate to the project directory:
    ```bash
    cd PythonPasswordGenerator
    ```

## Usage

1. Open the `password_generator.py` file in a text editor.

2. Run the script:
    ```bash
    python password_generator.py
    ```

## Example

The script generates a random password. By default, the password length is 10 characters. You can change the length by passing a different value to the `generate_password` function.

Example:
```python
import random
import string

def generate_password(length: int = 10):
    alphabet = string.ascii_letters + string.digits + string.punctuation
    password = ''.join(random.choice(alphabet) for i in range(length))
    return password

password = generate_password()
print(f"Generated Password: {password}")
