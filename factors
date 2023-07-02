#!/usr/bin/python3
Import time
import math
import sys

def pollard_rho(n):
    if n % 2 == 0:
        return 2
    
    x = 2
    y = 2
    d = 1 
    # Define the function f(x) using a lambda function
    f = lambda x: (x**2 + 1) % n
    # Loop until a non-trivial factor is found
    while d == 1:
        # Generate new values for x using the function f(x)
        x = f(x)
	
        # Generate new values for y using the function f(f(y))
        y = f(f(y))
        # Calculate the greatest common divisor between |x - y| and n
        d = math.gcd(abs(x - y), n)
    # Return the non-trivial factor
    return d

def main():
    # Check if the correct number of command-line arguments is provided
    if len(sys.argv) != 2:
        # Print the correct usage of the program
        print("Usage: python factorize.py <file>")
        # Exit the program if the correct arguments are not provided
        return
    # Get the file path from the command-line argument
    file_path = sys.argv[1]
    # start timing
    start_time = time.time()
    try:
        # Open the file in read mode
        with open(file_path, 'r') as file:
	# Read all lines of the file into a lis
            numbers = file.readlines()
        # Iterate through each number in the list
        for number in numbers:
	# Convert the string number to an integer
            num = int(number.strip())
	# Factorize the number using Pollard's rho algorithm
            factor = pollard_rho(num)
            # If the factor is equal to the original number
            if factor == num:
                # Print that the number is prime
                print(f"{num} is prime.")
            else:
	    # Print the factors of the number
                print(f"{num}={factor}*{num // factor}")

	if time.time() - start_time > 5:
                print("Time limit exceeded")
                exit()

    # Print an error message if the file is not found
    except FileNotFoundError:
        print(f"File '{file_path}' not found.")

if __name__ == '__main__':
    main()  # Call the main function when the script is executed

