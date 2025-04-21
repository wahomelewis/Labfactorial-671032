# Labfactorial-671032
# Factorial Calculator Program

def main():
    print("Welcome to the Factorial Calculation Program!")

    while True:
        try:
            num = int(input("Enter a non-negative integer to calculate its factorial: "))
            if num < 0:
                print("Factorial is not defined for negative numbers. Please try again.")
            else:
                break
        except ValueError:
            print("Invalid input. Please enter a valid non-negative integer.")

    factorial = 1
    for i in range(1, num + 1):
        factorial *= i

    print(f"The factorial of {num} is {factorial}")

if __name__ == "__main__":
    main()

