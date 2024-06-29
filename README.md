# note_app

# My Notes App - A Simple Note Taking Web App

This is a basic note-taking web application that allows you to create, view, delete, and edit notes.

# Features:

Add Notes: Write down your thoughts and ideas using the title and text fields provided.
View Notes: All your notes are displayed in a clear and organized manner.
Delete Notes: Easily remove notes you no longer need with a confirmation prompt.
Edit Notes: Modify existing notes by selecting them and making changes in the input fields.

# How to Use:

Open the HTML file in your web browser (e.g., Chrome, Firefox).
Enter a title and text for your note in the designated fields.
Click the "Add Note" button to save your note.
Your note will appear in the "Your Notes" section.
To delete a note, click the "Delete Note" button next to the corresponding note.
To edit a note, click the "Edit Note" button. Make your changes in the input fields and click "Add Note" again to save the edits.

# HTML:

Defines the basic structure of the app with a header for adding notes and a section for displaying existing notes.

# CSS:

Styles the various elements like headings, buttons, notes, etc., providing a clean and user-friendly interface.

# JavaScript:

Handles the interactivity of the app:
Listens for clicks on the "Add Note" button.
Validates if the note title and text are entered, displaying an alert if not.
Retrieves notes (if any) from local storage.
Creates a new note object with title and text from user input.
Stores the updated notes object back to local storage.
Clears the input fields after adding a note.
Defines a function showNotes to display existing notes:
Retrieves notes from local storage.
Iterates through each note and creates HTML elements dynamically.
Updates the "Your Notes" section with the generated HTML content or a message if there are no notes.
Defines functions for deleting and editing notes:
The deleteNote function takes the note index as input, confirms deletion with the user, removes the note from the notes object in local storage, and calls showNotes to update the display.
The editNote function takes the note index as input, retrieves notes from local storage, checks if the input fields are empty (to prevent overwriting unsaved edits), finds the note to edit based on the index, updates the note object with the current input values, removes the old note, stores the updated notes object back to local storage, and calls showNotes to update the display.
