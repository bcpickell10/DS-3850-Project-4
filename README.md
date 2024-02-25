# DS-3850-Project-4
This repository holds my class projects from DS 3850, which have been re-created with ChatGPT 3.5.

# Powerball
    import random
    import time

    def generate_powerball_numbers():
        input("Press Enter to generate Powerball numbers...")
    
    # Generating the first 5 numbers (1-69)
    numbers = sorted(random.sample(range(1, 70), 5))
    
    # Generating the Powerball number (1-26)
    powerball_number = random.randint(1, 26)
    
    print("Generating Powerball numbers...")
    time.sleep(1)
    
    # Displaying the numbers one at a time
    print("Powerball numbers are:")
    for num in numbers:
        print(num, end=" ", flush=True)
        time.sleep(1)
    print("\nPowerball:", powerball_number)  # Powerball number on its own line

    if __name__ == "__main__":
        generate_powerball_numbers()
