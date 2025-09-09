# Codenex
def Student_Grade_Calculator():
    marks = []
    for i in range(5):
        m=int(input("Enter marks for subjects : "))
        if 0 <= m <= 100:
            marks.append(m)
        else:
            print("Marks should be between 0 and 100")
    total_marks = sum(marks)
    average_marks = total_marks / 5
    grade = ""
    if average_marks >= 90:
        grade = "A"
    elif average_marks >= 75:
        grade = "B"
    elif average_marks >= 50:
        grade = "C"
    else:
        grade = "F"
    print("Total marks are",total_marks)
    print("Average marks are",average_marks)
    print("Your grade is",grade)
Student_Grade_Calculator()
