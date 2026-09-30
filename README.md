# PLC-based-conveyor-control
# PLC-Based Conveyor Control Simulation

conveyor = False

print("PLC-BASED CONVEYOR CONTROL")
print("--------------------------")

while True:
    print("\n1. START CONVEYOR")
    print("2. STOP CONVEYOR")
    print("3. OBJECT DETECTED")
    print("4. CONVEYOR STATUS")
    print("5. EXIT")

    choice = input("Enter your choice: ")

    if choice == "1":
        conveyor = True
        print("Conveyor STARTED")

    elif choice == "2":
        conveyor = False
        print("Conveyor STOPPED")

    elif choice == "3":
        if conveyor:
            print("Object detected by sensor.")
            print("Conveyor continues running.")
        else:
            print("Conveyor is stopped.")

    elif choice == "4":
        if conveyor:
            print("Conveyor STATUS: RUNNING")
        else:
            print("Conveyor STATUS: STOPPED")

    elif choice == "5":
        print("PLC system stopped.")
        break

    else:
        print("Invalid choice!")
        
