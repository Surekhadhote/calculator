from tkinter import *
import math


class calc:

    def getandreplace(self):
        self.expression = self.e.get()
        self.newtext = self.expression.replace('x','*')
   

    def equals(self,argi):
        self.getandreplace()

        try:
            self.value = eval(self.newtext)

        except SyntaxError or NameError:
            self.e.delete(0,END)
            self.e.insert(0,'invalid')

        else:
            self.e.delete(0,END)
            self.e.insert(0,self.value)


    def clearall(self):
        self.e.delete(0,END)


    def action(self,argi):
        self.e.insert(END,argi)


    def __init__(self,master):
        self.newtext = str(self)
        master.title("calculator")
        master.geometry()
        self.e = Entry(master,width = 35, fg="blue", bg="pink")
        self.e.grid(row=0,column=0,pady=3,padx=19,columnspan=20)
        self.e.focus_set()

        Button(master, text="=", width=11, height=3, command=lambda: self.equals('=')).grid(row=2,
                                                                                                               column=1,
                                                                                                               columnspan=3)
        Button(master, text="-", width=11, height=3, fg="blue", bg="pink", command=lambda: self.action('-')).grid(row=2,
                                                                                                               column=4,
                                                                                                               columnspan=3)
        Button(master, text="+", width=11, height=3, command=lambda: self.action('+')).grid(row=2,
                                                                                                               column=8,
                                                                                                               columnspan=3)
        Button(master, text="*", width=11, height=3, fg="blue", bg="pink", command=lambda: self.action('x')).grid(row=3,
                                                                                                               column=1,
                                                                                                               columnspan=3)
        Button(master, text="/", width=11, height=3, fg="blue", bg="pink", command=lambda: self.action('/')).grid(row=3,
                                                                                                               column=4,
                                                                                                               columnspan=3)
        Button(master, text="1", width=11, height=3, fg="blue", bg="pink", command=lambda: self.action('1')).grid(row=3,
                                                                                                               column=8,
                                                                                                               columnspan=3)
        Button(master, text="2", width=11, height=3, fg="blue", bg="pink", command=lambda: self.action('2')).grid(row=4,
                                                                                                               column=1,
                                                                                                               columnspan=3)
        Button(master, text="3", width=11, height=3,  command=lambda: self.action('3')).grid(row=4,
                                                                                                               column=4,
                                                                                                               columnspan=3)
        Button(master, text="4", width=11, height=3, fg="blue", bg="pink", command=lambda: self.action('4')).grid(row=4,
                                                                                                               column=8,
                                                                                                               columnspan=3)
        Button(master, text="5", width=11, height=3, fg="blue", bg="pink", command=lambda: self.action('5')).grid(row=5,
                                                                                                               column=1,
                                                                                                               columnspan=3)
        Button(master, text="6", width=11, height=3, fg="blue", bg="pink", command=lambda: self.action('6')).grid(row=5,
                                                                                                               column=4,
                                                                                                               columnspan=3)
        Button(master, text="8", width=11, height=3, fg="blue", bg="pink", command=lambda: self.action('8')).grid(row=5,
                                                                                                               column=8,
                                                                                                               columnspan=3)
        Button(master, text="7", width=11, height=3,  command=lambda: self.action('7')).grid(row=6,
                                                                                                               column=1,
                                                                                                               columnspan=3)
        Button(master, text="9", width=11, height=3, fg="blue", bg="pink", command=lambda: self.action('9')).grid(row=6,
                                                                                                               column=4,
                                                                                                               columnspan=3)
        Button(master, text="0", width=11, height=3,  command=lambda: self.action('0')).grid(row=6,
                                                                                                                  column=8,
                                                                                                                  columnspan=3)

        Button(master, text="AC",  command=lambda: self.clearall()).grid(row = 0,
                                                                                           column = 10,columnspan=1)

root = Tk()
obj = calc(root)
root.mainloop()

