from tkinter import *

window=Tk()
window.title("Login Screen")
window.geometry("500x500")

frame=Frame(master=window,height=300,width=460,bg='grey')

lbl1=Label(frame,text='User ID',bg='white',fg='black',width=12)
lbl2=Label(frame,text='Email',bg='white',fg='black',width=12)
lbl3=Label(frame,text='Password',bg='white',fg='black',width=12)

identry=Entry(frame)
emailentry=Entry(frame)
passwordentry=Entry(frame, show='*')

def display():
    name=identry.get()
    greet="Welcome " + name
    message="\n Login Successful"
    textbox.insert(END,greet)
    textbox.insert(END,message)

textbox=Text(bg='white', fg='black')

btn=Button(text="Login",command=display,bg='white')

frame.place(x=20,y=0)
lbl1.place(x=40,y=80)
identry.place(x=150,y=80)
lbl2.place(x=40,y=120)
emailentry.place(x=150,y=120)
lbl3.place(x=40,y=160)
passwordentry.place(x=150,y=160)
btn.place(x=130,y=210)
textbox.place(y=250)


window.mainloop()