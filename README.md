# INTERACTIVE-CALCULATOR-UNIT-CONVERTER-

# PROJECT 01: INTERACTIVE CALCULATOR & UNIT CONVERTER

def calculator():
    print("\n--- Arithmetic Calculator ---")
    print("1. Addition")
    print("2. Subtraction")
    print("3. Multiplication")
    print("4. Division")

    choice = int(input("Enter your choice: "))

    a = float(input("Enter first number: "))
    b = float(input("Enter second number: "))

    if choice == 1:
        print("Result =", a + b)
    elif choice == 2:
        print("Result =", a - b)
    elif choice == 3:
        print("Result =", a * b)
    elif choice == 4:
        if b != 0:
            print("Result =", a / b)
        else:
            print("Cannot divide by zero!")
    else:
        print("Invalid choice")


def currency_converter():
    print("\n--- Currency Converter ---")
    print("1. INR to USD")
    print("2. USD to INR")

    choice = int(input("Enter your choice: "))
    amount = float(input("Enter amount: "))

    if choice == 1:
        print("USD =", amount / 88)
    elif choice == 2:
        print("INR =", amount * 88)
    else:
        print("Invalid choice")


def unit_converter():
    print("\n--- Unit Converter ---")
    print("1. Kilometers to Meters")
    print("2. Meters to Kilometers")
    print("3. Kilograms to Grams")
    print("4. Grams to Kilograms")

    choice = int(input("Enter your choice: "))
    value = float(input("Enter value: "))

    if choice == 1:
        print("Meters =", value * 1000)
    elif choice == 2:
        print("Kilometers =", value / 1000)
    elif choice == 3:
        print("Grams =", value * 1000)
    elif choice == 4:
        print("Kilograms =", value / 1000)
    else:
        print("Invalid choice")


# Main Program
while True:
    print("\n===== MAIN MENU =====")
    print("1. Calculator")
    print("2. Currency Converter")
    print("3. Unit Converter")
    print("4. Exit")

    choice = int(input("Enter your choice: "))

    if choice == 1:
        calculator()
    elif choice == 2:
        currency_converter()
    elif choice == 3:
        unit_converter()
    elif choice == 4:
        print("Thank you for using the program!")
        break
    else:
        print("Invalid choice! Try again.")
