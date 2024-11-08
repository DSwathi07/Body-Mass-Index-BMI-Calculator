import random

# Function to simulate a dice roll
def roll_dice():
    # Generate a random number between 1 and 6
    roll = random.randint(1, 6)
    return roll

# Main program to run the dice roll simulation
if __name__ == "_main_":
    print("Welcome to the Dice Roll Simulator!")
    
    # Ask user if they want to roll the dice
    while True:
        input("Press Enter to roll the dice...")

        # Roll the dice
        roll_result = roll_dice()
        
        # Display the result of the roll
        print(f"The dice rolled: {roll_result}")
        
        # Ask if the user wants to roll again
        roll_again = input("Do you want to roll again? (yes/no): ").lower()
        if roll_again != "yes":
