# Password_pop_up

import tkinter as tk
from tkinter import simpledialog
from tkinter import messagebox

def show_popup():
    user_input = simpledialog.askstring("Input", "Please enter your password:")
    
    setpassword = "HELLO"
    
    if user_input == setpassword:
        messagebox.showinfo("Popup", "Password is correct!")
    else:
        messagebox.showinfo("Password", "Incorrect password.")

# Create the main window
root = tk.Tk()
root.title("    ")

# Create a button that triggers the popup
button = tk.Button(root, text="Click me!", command=show_popup)
button.pack(pady=20)

# Run the application
root.mainloop()

