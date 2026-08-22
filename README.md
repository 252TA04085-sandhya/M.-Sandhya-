students = {}

while True:
    print("\n1. Add Student")
    print("2. View Students")
    print("3. Exit")

    choice = input("Enter choice: ")

    if choice == "1":
        name = input("Enter name: ")
        marks = float(input("Enter marks: "))
        students[name] = marks
        print("Student added!")

    elif choice == "2":
        for name, marks in students.items():
            print(name, ":", marks)

    elif choice == "3":
        print("Program ended")
        break

    else:
        print("Invalid choice")
