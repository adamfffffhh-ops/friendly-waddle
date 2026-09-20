# ============================================
#        BIG HELLO WORLD PYTHON PROGRAM
# ============================================

import time
import sys
import random

# ---------- Configuration ----------
MESSAGE = "Hello World!"
AUTHOR = "Python"

# ---------- Simple print ----------
print(MESSAGE)

# ---------- Print letter by letter ----------
print("\nLetter by letter:")

for letter in MESSAGE:
    print(letter, end="", flush=True)
    time.sleep(0.1)

print("\n")

# ---------- Repeating ----------
print("Repeating message:")

for i in range(5):
    print(f"{i + 1}: {MESSAGE}")

# ---------- ASCII-style box ----------
print("\nASCII Box:")
print("+" + "-" * 30 + "+")
print("|" + MESSAGE.center(30) + "|")
print("+" + "-" * 30 + "+")

# ---------- Big text ----------
print("\nBIG TEXT:")
print("""
██╗  ██╗███████╗██╗     ██╗      ██████╗
██║  ██║██╔════╝██║     ██║     ██╔═══██╗
███████║█████╗  ██║     ██║     ██║   ██║
██╔══██║██╔══╝  ██║     ██║     ██║   ██║
██║  ██║███████╗███████╗███████╗╚██████╔╝
╚═╝  ╚═╝╚══════╝╚══════╝╚══════╝ ╚═════╝

        H E L L O   W O R L D !
""")

# ---------- Random greeting ----------
greetings = [
    "Hello World!",
    "Hello Python!",
    "Welcome!",
    "Greetings from Python!",
    "Python says Hello!"
]

print("Random greeting:")
print(random.choice(greetings))

# ---------- Function ----------
def say_hello(name):
    return f"Hello {name}!"

print("\nUsing a function:")
print(say_hello("World"))

# ---------- Class ----------
class HelloWorld:
    def __init__(self, message):
        self.message = message

    def display(self):
        print(self.message)

hello = HelloWorld("Hello World from a Python class!")

print("\nUsing a class:")
hello.display()

# ---------- Countdown ----------
print("\nFinal countdown:")

for number in range(3, 0, -1):
    print(number)
    time.sleep(0.5)

print("\n" + "=" * 40)
print("        HELLO WORLD!")
print("=" * 40)

# ---------- Finish ----------
print("\nProgram finished successfully.")
