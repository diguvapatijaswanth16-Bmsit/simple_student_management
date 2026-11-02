students=[]
class student:
    def information(self):
        name=input("please enter the name:\n")
        usn=input("please enter your usn number:\n")
        mark1=int(input("please enter your maths marks:\n"))
        mark2=int(input("please enter your chemistry marks:\n"))
        mark3=int(input("please enter your ESC marks:\n"))
        mark4=int(input("please enter your ICO marks:\n"))
        mark5=int(input("please enter your ETC marks:\n"))
        mark6=int(input("please enter your python marks:\n"))
        avg_marks=((mark1*4)+(mark2*4)+(mark3*3)+(mark4*0)+(mark5*3)+(mark6*4))/6
        student=[name,usn,avg_marks]
        students.append(student)
    def display(self):
        for i in students:
            print(f"name:{i[0]}\nusn:{i[1]}\n marks{i[2]}")
a=student()
while True:
    a.required=input("a-add student,d-display students,e-exit")
    if a.required=="a":
        a.information()
    elif a.required=="d":
        a.display()
    elif a.required=="e":
        break
    else:
        print("this input does not exists")
