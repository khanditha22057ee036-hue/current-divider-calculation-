# Current Divider Calculation
# For two parallel resistors

Itotal = float(input("Enter total current (A): "))
R1 = float(input("Enter resistance R1 (Ohms): "))
R2 = float(input("Enter resistance R2 (Ohms): "))

if R1 <= 0 or R2 <= 0:
    print("Resistance must be greater than zero.")
else:
    I1 = Itotal * R2 / (R1 + R2)
    I2 = Itotal * R1 / (R1 + R2)

    print("Current through R1 =", round(I1, 2), "A")
    print("Current through R2 =", round(I2, 2), "A")