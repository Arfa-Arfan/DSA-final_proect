# Undo/Redo Program using Stack Data Structure

## 📌 Description
A Python-based text editor implementation demonstrating undo/redo functionality using the Stack (LIFO) principle, featuring multi-document support and an interactive CLI.

## 🎯 Project Overview
This project implements a robust undo/redo mechanism for text editing operations using the stack data structure. It allows users to track changes across multiple documents simultaneously and navigate through their edit history seamlessly.

## ✨ Features
- **Multi-document Management**: Create and switch between multiple text documents
- **Undo/Redo Functionality**: Step back (undo) and forward (redo) through edit history
- **Stack-based Architecture**: Uses LIFO principle for history management
- **Interactive CLI**: User-friendly command-line interface
- **Various Text Operations**:
  - Write/append text
  - Set/replace entire content
  - Clear document
  - Backspace/delete characters
  - Insert at specific position
  - Replace ranges
  - Replace all occurrences

## 🛠️ Technologies Used
- **Language**: Python 3.x
- **Data Structure**: Stack (using Python lists)
- **IDE**: Jupyter Notebook
- **Libraries**: re (command parsing), typing (type hinting)

## 📁 Project Structure
```
├── UndoRedoProject.ipynb    # Main Jupyter notebook with implementation
├── Undo_Redo_Project_Report.docx  # Detailed project report
└── README.md                 # Project documentation
```

## 🚀 How to Run
1. Open `UndoRedoProject.ipynb` in Jupyter Notebook
2. Run Cell 1 to define the `UndoRedo` class
3. Run Cell 3 to define the editor and commands
4. Run Cell 5 to define the interactive loop
5. Run Cell 6 to start the CLI

## 💻 Available Commands
```
new <name>            # Create and switch to a new document
use <name>            # Switch to document (creates if missing)
list                  # List all documents
write <text>          # Append text to the end
set <text>            # Replace entire content
clear                 # Erase entire content
backspace [n]         # Delete last n chars (default 1)
delete [n]            # Alias of backspace
insertat <pos> <text> # Insert at specific index
replaceat <pos> <len> <text>  # Replace range
replaceall <old> <new> # Replace all occurrences
show                  # Display current content
undo                  # Undo last change
redo                  # Redo last undone change
next                  # Show next write index
help                  # Display help
exit                  # Quit program
```

## 🧠 Key Concepts Demonstrated
- **Last-In-First-Out (LIFO)** principle
- Stack operations: push and pop
- State management with undo/redo stacks
- Multi-document architecture
- Command pattern implementation

## 📊 How It Works
1. **State Capture**: Before any edit, current text is pushed to undo_stack
2. **Execution**: Text modification is performed
3. **Redo Invalidation**: redo_stack is cleared after new edits
4. **Undo**: Pops from undo_stack and pushes current state to redo_stack
5. **Redo**: Pops from redo_stack and pushes current state to undo_stack

## 🎓 Learning Outcomes
- Practical application of stack data structure
- Understanding of undo/redo mechanisms in software
- Multi-document state management
- Command-line interface design
- Python class design and inheritance

## 📝 Author
**Arfa Arfan**  
Roll No: 2024-Csre-032  
BS Computer Science (3rd Semester)  
University of Veterinary & Animal Sciences, Ravi Campus, Pattoki

## 👨‍🏫 Instructor
**Mr. Azeem Aslam**  
Course: Data Structures and Algorithms

## 📅 Project Timeline
- Topic Selection & Proposal: Week 1
- System Design: Week 2
- Basic Text Handling: Week 3
- Undo Functionality: Week 4
- Redo Functionality: Week 5
- Debugging & Testing: Week 6
- Report Preparation: Week 7
- Final Demo: Week 8

## 🔗 References
- Python Software Foundation. *Data Structures: Using Lists as Stacks*
- Project Implementation: UndoRedoProject.ipynb
