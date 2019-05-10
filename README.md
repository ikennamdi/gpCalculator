# gpCalculator

print("\n		WELCOME TO GRADE POINT AVERAGE CALCULATOR\n")

studentName = str(input("Enter Your Name: "))

print("\nHello " + studentName + "... Let's Calculate your Grade Point Average.\n(Click \"Enter\" to continue)")

gPoint = 0
tPoint = 0
cUnit = 0
tUnit = 0
cgpa = 0
task = True

while True:
    print('\n**********Enter "END" to end program**********\n          (Case Sensitive)')

    cTitle = str(input("\nEnter Your Course Title: "))
    if cTitle == "END":
        break

    cUnit = int(input("Enter Course Unit: "))

    grade = [5, 4, 3, 2, 1, 0]

    cGrade = str(input("Enter Course Grade: "))

    if cGrade == "A" or cGrade == "a":
        gPoint = (5 * cUnit)

    if cGrade == "B" or cGrade == "b":
        gPoint = (4 * cUnit)

    if cGrade == "C" or cGrade == "c":
        gPoint = (3 * cUnit)

    if cGrade == "D" or cGrade == "d":
        gPoint = (2 * cUnit)

    if cGrade == "E" or cGrade == "e":
        gPoint = (1 * cUnit)

    if cGrade == "F" or cGrade == "f":
        gPoint = (0 * cUnit)


    tPoint = tPoint + gPoint
    tUnit = tUnit + cUnit

    print("\nCourse        Unit    TotalUnit    GradePoint    TotalGradePoint")
    print(cTitle, "          ", cUnit, "          ", tUnit, "          ", gPoint, "          ", tPoint)

    cgpa = tPoint / tUnit
    print("\nCGPA: ", "%.2f" % cgpa)


print('\nBreaking....................')
print('Closing Program...........')
print('Program Closed!')




