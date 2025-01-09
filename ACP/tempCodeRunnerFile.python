from tkinter import *
from datetime import date
from datetime import datetime

window = Tk()
window.title("Age Calculator")
window.geometry("500x500")

frame = Frame(master=window, height=300, width=460, bg='grey')

lbl1 = Label(frame, text='Name', bg='white', fg='black', width=12)
lbl2 = Label(frame, text="Birthday (YYYY-MM-DD)", bg='white', fg='black', width=20)

nameentry = Entry(frame)
ageentry = Entry(frame)

def display():
    name = nameentry.get()
    birthdate_str = ageentry.get()
    try:
        birthdate = datetime.strptime(birthdate_str, '%Y-%m-%d')
        age = calculateAge(birthdate)
        greet = f"Welcome {name}\nYour age is {age} years."
    except ValueError:
        greet = "Invalid date format. Please enter in YYYY-MM-DD format."
    
    textbox.delete("1.0", END)
    textbox.insert(END, greet)

def calculateAge(birthDate):
    today = date.today()
    age = today.year - birthDate.year - ((today.month, today.day) < (birthDate.month, birthDate.day))
    return age

textbox = Text(bg='white', fg='black', height=4, width=50)

btn = Button(text="Calculate", command=display, bg='white')

frame.place(x=20, y=0)
lbl1.place(x=40, y=80)
nameentry.place(x=200, y=80)
lbl2.place(x=40, y=140)
ageentry.place(x=200, y=140)
btn.place(x=180, y=210)
textbox.place(y=250, x=20)

window.mainloop()
