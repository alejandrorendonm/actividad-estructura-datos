# Copilot Instructions for actividad-estructura-datos

## Project Overview
This is a simple Java console application implementing a text editor with undo/redo functionality. The main logic resides in `src/TextEditor.java`.

## Architecture & Data Flow
- The application is single-file (`TextEditor.java`) and uses two `Stack<String>` objects for undo/redo operations.
- User interaction is via a console menu loop.
- All text additions are pushed to the undo stack; redo stack is intended for future use (currently not implemented).

## Developer Workflows
- **Run the app:**
  - Compile: `javac src/TextEditor.java`
  - Run: `java -cp src TextEditor`
- **No build system or tests** are present; all logic is in the main method.

## Project-Specific Patterns
- **Menu-driven input:** All user actions are handled via numbered menu options.
- **Undo/Redo stacks:** Use Java's `Stack` for managing text history. Undo/redo logic should push/pop strings as appropriate.
- **UTF-8 input:** Scanner is initialized with UTF-8 encoding for international text support.

## Conventions
- All code is in `src/TextEditor.java`.
- No external dependencies or frameworks.
- No package declarations; everything is in the default package.

## Examples
- To add undo/redo logic, manipulate `undoStack` and `redoStack` in the switch statement.
- To extend functionality, add new menu options and handle them in the main loop.

## Key File
- `src/TextEditor.java`: Main application logic and entry point.

---

If you add new files or features, update this document to reflect new patterns or workflows.
