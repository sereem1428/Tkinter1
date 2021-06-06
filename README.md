from tkinter import *
from tkinter import ttk

window = Tk()
window.geometry('400x400+400+200')
month = StringVar()
year = StringVar()
lb = Label(window, text='what is your birth month ?', ).pack()
cb = ttk.Combobox(window, values=("Jaan", "Feb", "Mar"),
                  textvariable=month
                  )
cb.pack()
lb = Label(window, text='what is your birth year ?').pack()
cb = ttk.Combobox(window, values=("2006", "2007", "2008", "2009"),
                  textvariable=year
                  )
cb.pack()
bt = Button(window, text='show')
window.mainloop()
