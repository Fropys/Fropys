import tkinter as tk

root = tk.Tk()
root.title('counting second')
window_width = 300
window_height = 200

message = tk.Label(root, text="Hai Kesayanganku")
message.pack()


#Get the screen dimension
screen_widht = root.winfo_screenmmwidth()
screen_height = root.winfo_screenmmheight()

#find the center point
center_x = int(screen_widht/2 - window_width / 2)
center_y = int(screen_height/2 - window_height / 2)

#set the position of the window to the center of the screen
root.geometry(f'{window_width}x{window_height}+{center_x}+{center_y}')

button = tk.Button (root, text = 'Klik Disini', width=10,height=2, command=root.destroy) 

# set button position
button.place(x=110, y=100)
root.mainloop() 

# Import the required libraries
from tkinter import *
from tkinter import messagebox
from tkinter import ttk

# Create an instance of tkinter frame
win= Tk()
# Set the size of the tkinter window
win.geometry("700x350")


def show_msg():
 messagebox.showinfo("I Love U So Much") 
 
# Add an optional Label widget
Label(win, text= "Klik Di Bawah", font= ('Aerial 17 bold italic')).pack(pady= 30)
# Create a Button to display the message
ttk.Button(win, text= "Sekali Lagi",command=show_msg).pack(pady= 20)

win.mainloop() 
