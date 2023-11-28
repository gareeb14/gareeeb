# gareeeb
using python.Creating aviator bot.
import random

def choose_multiplier():
    multiplier = random.uniform(1.2, 30)
    if multiplier > 5:
        # Adjusting probability for numbers over 5
        if random.random() < 0.3:  # Adjust probability as needed
            multiplier = random.uniform(1.2, 5)
    return multiplier

def choose_number():
    number = random.randint(1, 30)
    if number > 15:
        # Adjusting probability for numbers over 15
        if random.random() < 0.2:  # Adjust probability as needed
            number = random.randint(1, 15)
    return number

multiplier = choose_multiplier()
number = choose_number()

print("Multiplier:", multiplier)
print("Number:", number)
