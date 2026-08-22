num = int(input("Enter a number: "))

digits = len(str(num))
total = sum(int(digit) ** digits for digit in str(num))

if total == num:
    print("Armstrong Number")
else:
    print("Not Armstrong Number")
