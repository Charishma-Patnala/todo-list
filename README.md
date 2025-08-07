# todo-list
Create a To-Do List Application (Console-based) Objective: Implement a simple to-do list manager. Tools :Python, VS Code / terminal. Deliverables: Python file (todo.py). Hints/Mini Guide: 1.Use lists to store tasks 2.Implement add/remove/view functionality 3.Store tasks in a text file using open() Outcome: Persistent CLI to-do app.
How the Program Works
File Handling (load_tasks, save_tasks):
The program uses a file named tasks.txt to store your to-do items.
load_tasks() reads from this file when the application starts. This ensures your tasks are not lost when you close the program. If the file doesn't exist, it starts with an empty list.
save_tasks() writes the current list of tasks back to the file every time you add or remove an item, ensuring persistence.
Core Functions (view_tasks, add_task, remove_task):
view_tasks: Simply prints the current list of tasks with numbers, making it easy to see what you need to do.
add_task: Prompts you to enter a new task and adds it to the list.
remove_task: Shows you the list and asks for the number of the task you want to delete. It includes error handling to prevent crashes if you enter text or an invalid number.
Main Loop (main):
This function acts as the control center. It first loads any existing tasks.
It then enters an infinite loop that displays the menu and waits for your input (1, 2, 3, or 4).
Based on your choice, it calls the appropriate function. The loop breaks only when you choose option 4 to exit.
