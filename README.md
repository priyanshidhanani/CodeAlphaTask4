# Simple Chatbot in Python

## Overview

This project is a basic rule-based chatbot written in Python. It responds to a few predefined user inputs and continues the conversation until the user types `bye`.

---

## Code Explanation (Line by Line)

### Function Definition

```python
def chatbot_response(user_input):
```

* Defines a function named `chatbot_response`.
* The function accepts one parameter: `user_input`.

```python
user_input = user_input.lower()
```

* Converts the user's input to lowercase.
* This makes the chatbot case-insensitive.
* Example: `"HELLO"` becomes `"hello"`.

---

### Greeting Response

```python
if user_input == "hello":
    return "Hi!"
```

* Checks whether the user entered `"hello"`.
* If true, the chatbot responds with `"Hi!"`.

---

### How Are You Response

```python
elif user_input == "how are you":
    return "I'm fine, thanks!"
```

* Checks if the user asks `"how are you"`.
* Returns a friendly response.

---

### Name Response

```python
elif user_input == "what is your name":
    return "I am a simple chatbot."
```

* Checks if the user asks for the chatbot's name.
* Returns a predefined answer.

---

### Exit Response

```python
elif user_input == "bye":
    return "Goodbye!"
```

* Checks whether the user wants to end the conversation.
* Returns a goodbye message.

---

### Default Response

```python
else:
    return "Sorry, I don't understand that."
```

* Executes when none of the previous conditions match.
* Handles unknown inputs.

---

## Program Header

```python
print("===== SIMPLE CHATBOT =====")
```

* Displays the chatbot title.

```python
print("Type 'bye' to exit.\n")
```

* Shows instructions for the user.

---

## Infinite Loop

```python
while True:
```

* Starts an infinite loop.
* The chatbot continues running until manually stopped.

---

## User Input

```python
user = input("You: ")
```

* Takes input from the user.
* Stores it in the variable `user`.

---

## Get Chatbot Response

```python
response = chatbot_response(user)
```

* Sends the user's message to the function.
* Stores the returned response.

---

## Display Response

```python
print("Bot:", response)
```

* Prints the chatbot's reply.

---

## Exit Condition

```python
if user.lower() == "bye":
    break
```

* Checks if the user entered `"bye"`.
* `break` stops the loop and ends the program.

---

## Sample Run

```text
===== SIMPLE CHATBOT =====
Type 'bye' to exit.

You: hello
Bot: Hi!

You: how are you
Bot: I'm fine, thanks!

You: what is your name
Bot: I am a simple chatbot.

You: bye
Bot: Goodbye!
```

---

## Concepts Used

* Functions
* Parameters
* Strings
* Conditional Statements (`if`, `elif`, `else`)
* Loops (`while`)
* User Input (`input`)
* Output (`print`)
* String Methods (`lower()`)

---

## Conclusion

This chatbot is a beginner-friendly Python project that demonstrates how to use functions, loops, conditions, and user input to create a simple conversational program.
