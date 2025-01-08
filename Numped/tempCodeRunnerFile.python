from tkinter import *

root=Tk()
root.title("Number Pad")
root.geometry("500x500")

nump=[1,2,3],[4,5,6],[7,8,9],['#',0,'*']

for i in range(4):
    root.columnconfigure(i,weight=1,minsize=150)
    root.rowconfigure(i,weight=1,minsize=85)

for i in range(4):
    for j in range(3):
        frame=Frame(master=root,relief=GROOVE,borderwidth=4,bg='pink')
        frame.grid(row=i, column=j,sticky="nsew")

        label=Label(master=frame,text=nump[i][j],bg='lightblue',font=("Times New Roman", 10))
        label.pack(expand=True,fill="both", padx=5,pady=5)

root.mainloop()