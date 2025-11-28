# pthyon_mini_project
import random

def roll_dice():
    """Simulates rolling a single six-sided die."""
    # Generate a random number between 1 and 6
    roll = random.randint(1, 6)
    print(f"\nRolled: {roll}")

# Main program loop
while True:
    user_input = input("Roll the dice? (yes/no): ").lower().strip()
    
    if user_input == 'yes' or user_input == 'y':
        roll_dice()
    elif user_input == 'no' or user_input == 'n':
        print("Goodbye!")
        break
    else:
        print("Invalid input. Please enter 'yes' or 'no'.")
