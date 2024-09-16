# Python | Palindrome Checker
**Objective:** Develop a Python script that checks if a string is a palindrome, with an interactive feature for repeated user input.

### Requirements:

| **Requirement**         | **Description**                                                                                          |
|-------------------------|----------------------------------------------------------------------------------------------------------|
| **Palindrome Check**    | Implement a function to check if a string reads the same forward and backward, ignoring spaces, punctuation, and capitalization. |
| **User Interaction**    | Prompt the user to enter a word or phrase to check if it's a palindrome. Display the result and prompt again automatically. |
| **Loop and Exit Option**| Continuously ask for user input in a loop. Provide an option for the user to exit the loop (e.g., by typing "exit" or "quit"). |
| **Usability**           | Ensure the script is user-friendly with clear instructions on how to enter text and exit the program. Aim for simplicity and efficiency. |

### My Python Code:

```python
import string

def is_palindrome(s: str) -> bool:
    # Convert to lowercase and remove spaces, punctuation
    cleaned_str = ''.join(char.lower() for char in s if char.isalnum())
    
    # Check if the cleaned string reads the same forward and backward
    return cleaned_str == cleaned_str[::-1]

# Loop to continuously ask for user input
while True:
    # Ask the user for input
    user_input = input("What word or phrase do you want to check for a palindrome? (or type 'exit' to quit): ")
    
    # Check if the user wants to exit
    if user_input.lower() == 'exit':
        print("Exiting the palindrome checker. Goodbye!")
        break

    # Check if the input is a palindrome and print the result
    if is_palindrome(user_input):
        print(f'"{user_input}" is a palindrome!')
    else:
        print(f'"{user_input}" is not a palindrome.')
```
### Result:
![image](https://github.com/user-attachments/assets/4f86a362-af7d-439e-a5aa-31c7f61819c6)

Please download my attached file for testing purpose

Thank you for stopping by, and I'm pleased to connect with you, my new friend!

**Please do not forget to FOLLOW and star ⭐ the repository if you find it valuable.**

Wish you a day filled with happiness and energy!

Warm regards,

Hien Moon | [Visit My Blog](https://hienmoon.com/?utm_source=github&utm_medium=readme)
