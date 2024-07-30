# Module2-MiniProject
 To-Do List Application

This application is meant to help you manage a To-Do List!

Once you run the code, the application will start up with a welcome message.

It will give you a menu with options to choose from.

You can:
    1. Add a task.
        ~ You will be prompted to "Enter the title of the task to add: ".
        ~ The program will then check if the task's title you have entered already exists.
            - If not, it will add the task to your to-do list with a default status of "Incomplete" and advises you "Task 'task you enter' has been added.".
            - If it does, it will advise you: "The task 'task you enter' already exists.".
    2. View the tasks.
        ~ This option will provide you a user-friendly version of your to-do list.
        ~ Including:
            - "Your To-Do List:" Header
            - Each of your tasks with their corresponding statuses
    3. Mark a task as complete.
        ~ You will be prompted to "Enter the title of the task you would like to mark as complete: ".
        ~ The program will check if the task's title you have entered exists.
            - If it exists, the program will move to the next step.
            - If it does not exist, it will advise you: "Task 'task you enter' does not exist."
        ~ The program will then check if the task's title that you entered is already marked as complete.
            - If the status is not currently "complete", it will mark the task as complete and advise you "The task 'task you enter' is now marked complete.".
            - If the status is already marked as "complete", it will advise you: "Task 'task you enter' is already complete.".
    4. Delete a task.
        ~ You will be prompted to "Enter the title of the task you would like to delete: ".
        ~ The program will then check if the task's title you have entered does not exist in the current list.
            - If it does not exist, it advises you "Task 'task you enter' does not exist.".
            - If it does exist, it will remove the task and advise you "Your task 'task you enter' has been deleted.".
    5. Quit the program.
        ~ This will advise you "Quiting the program..." and stops the program from running further.
    * After each choice you make and complete, the program will also thank you for using the To-Do List app!

Error Handling:

This program has a few built-in error exceptions to ensuring proper handling of potential errors that may occur.

These include:
    1. ValueError exception:
        ~ To ensure the proper value is inputted for the choice selection by the user.
        ~ Provides the user an error message stating: "That is not a valid choice. Please enter the digit that corresponds with your selection."
    2. TypeError exception:
        ~ To ensure if any unexpected errors occur the user will be prompted with: "An unexpected type error occurred. Please ensure you enter the digit that corresponds with your selection."
    3. Checks on user inputs:
        - checks if the user's input is empty and if so, reprompts the user for input
        - checks if the user's input for tasks' titles does or does not exists
        - checks if the user's input for task to be marked as complete is already complete
        - takes user's inputs and converts to lower case for ease of functionality
        - in functions, for strings converts them to have first letter capitalized for ease of functionality and user-friendly viewing