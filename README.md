import time

def main():
    print("Welcome to Chandrayaan 2 Landing Simulation!")
    time.sleep(1)

    altitude = 10000  # Starting altitude in meters

    while altitude > 0:
        print(f"Altitude: {altitude} meters")
        action = input("Enter 'b' to burn thrusters or 'c' to cut power: ")

        if action == 'b':
            altitude -= 1000  # Simulate a controlled burn
        elif action == 'c':
            altitude -= 500  # Simulate power cut
        else:
            print("Invalid input. Choose 'b' or 'c'.")

    print("Landing successful!")

if __name__ == "__main__":
    main()
