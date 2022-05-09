# first_dictionary.py

from microbit import *

sleep(1000)

string = input("Enter your name: ")

text = input("Enter a recent game score: ")
value = int(text)

info = {   }

info['name'] = string
info['score'] = value

print("Dictionary")
print("info = ", info)

name_val = info['name']
text = info['score']
score_val = int(text)

print("Hello", name_val, "your score was", score_val)

print("Enter game high score instead: ")
text = input("Enter high score: ")
value = int(text)

info['score'] = value

print("Updated dictionary: ")
print("info = ", info)

text = input("Enter score to reach next week: ")
value = int(text)

info['goal'] = value

print("Updated dictionary")
print("info = ", info)

text = info['score']
score = int(text)

text = info['goal']
score_goal = int(text)

difference = score_goal - score

print("That's", difference, "points more.")