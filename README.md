# yuyaya19.github.com
Just another repository
#!/usr/bin/python 
# -*- coding: gbk -*- 

import requests
import io 
import sys 
sys.stdout = io.TextIOWrapper(sys.stdout.buffer,encoding='gb18030')
from tkinter import *
from PIL import Image,ImageTk
import tkinter
import tkinter.messagebox
root=Tk()
root.title('xiao')
root.geometry("731x411+100+100")
cv= Canvas(root, width = 731, height =411, bg = "black") 
cv.pack()
frame = Frame(root) 
frame.pack() 
image = Image.open("21.jpg")
im = ImageTk.PhotoImage(image) 
cv.create_image(367,206,image = im) 
def showDialogNO():
   tkinter.messagebox.showinfo(title='伤心了', message='余亚飞不想说') 
def showDialogOK():
   tkinter.messagebox.showinfo( title="中文版", message="祝余亚飞生日快乐！") 
   tkinter.messagebox.showinfo( title="英文版", message="Happy birthday to my yuyafei!") 
   tkinter.messagebox.showinfo(title="日语版", message="私の余亚飞の誕生日おめでとうございます!") 
   tkinter.messagebox.showinfo(title="GGN版", message="余亚亚，生日快乐!高考加油哦！愿心之所向皆可成。") 
   root.destroy() 
def showDialogEE(): 
   tkinter.messagebox.showinfo(title='错了吗', message='那我明天再来')
def closeWindow(): 
   tkinter.messagebox.showerror(title='未作回应',message='哼，关掉也没用!') 
   return
root.protocol('WM_DELETE_WINDOW', closeWindow) 
output_label0 = Label(root,text ="余亚亚，生日快乐?", font =("仿宋", 18,"")) 
cv.create_window(280, 20, anchor=NW, window= output_label0)
Button1 = Button(root, text="是", font =("仿宋", 18,"bold"),width=8,height=1,command = showDialogOK)
cv.create_window(130, 360, anchor=NW, window=Button1)
Button2 = Button(root,text='不是', font =("仿宋", 18,"bold"),width=8,height=1,command = showDialogEE) 
cv.create_window(300, 360, anchor=NW, window=Button2) 
Button3 = Button(root,text='我想想', font =("仿宋", 18,"bold"),width=8,height=1,command = showDialogNO)
cv.create_window(470, 360, anchor=NW, window=Button3)
root.mainloop() 




