🧮 Command-Line Calculator

A simple yet powerful GUI calculator built with Bash and Zenity that provides an intuitive graphical interface for performing basic arithmetic operations in Linux environments. It bridges the gap between command-line efficiency and user-friendly graphical interaction.

🧩 Project Overview

The Command-Line Calculator allows users to:
Perform basic arithmetic operations (Addition, Subtraction, Multiplication, Division) through graphical dialog boxes.
Enter numeric inputs (integers and decimals) with visual prompts.
Select operations from an interactive list-based menu.
Receive instant calculation results with error validation.

🎯 Objectives

Build a user-friendly calculator with GUI elements for Linux systems.
Demonstrate bash scripting proficiency with control structures and external tool integration.
Implement robust error handling for division by zero and invalid inputs.
Practice shell scripting concepts using Zenity, bc, and conditional logic.

⚙️ Functional Overview

Feature	Description
Graphical Input	Uses Zenity dialog boxes for user-friendly number entry
Operation Selection	Interactive list menu for choosing arithmetic operations
Precision Calculations	Leverages GNU bc for accurate floating-point arithmetic (up to 10 decimal places)
Error Handling	Validates division by zero and handles user cancellations gracefully
Result Display	Shows calculation results in a clean information dialog

🧠 Core Components

Data Structures
Variables: num1, num2 — Store user-input numbers
Operation Variable: operation — Stores selected arithmetic operator (+, -, *, /)
Result Variable: result — Stores calculated output

Key Functions

Function	Purpose
zenity --entry	Creates text input dialogs for number entry
zenity --list	Displays operation selection menu
zenity --info	Shows the final calculation result
zenity --error	Displays error messages for invalid operations
bc -l	Performs precise arithmetic calculations
case statement	Routes operations to appropriate calculation logic

💻 How It Works

First Input: The program prompts the user to enter the first number via a dialog box.
Second Input: The user enters the second number through another dialog.
Operation Selection: A list menu displays all available operations (+, -, *, /).
Calculation: Based on the selected operation, the script uses bc to compute the result.
Result Display: The final answer is shown in an information dialog.
Error Handling: If division by zero is attempted, an error dialog appears.

🔧 Installation

Prerequisites
Before running the calculator, ensure you have the following installed:
Bash (v5.x or higher)
Zenity (v3.x or higher)
bc (GNU Basic Calculator)
Linux OS (Ubuntu, Debian, Fedora, Arch, etc.)
X11 Display Server (for GUI dialogs)

Installation Steps
For Debian/Ubuntu:

bash
sudo apt-get update
sudo apt-get install zenity bc
For Fedora:

bash
sudo dnf install zenity bc
For Arch Linux:

bash
sudo pacman -S zenity bc
Make Script Executable
bash
chmod +x calculator.sh

🚀 Usage

Running the Calculator
bash
./calculator.sh
Or run it directly with bash:

bash
bash calculator.sh
Example Workflow
First Input: Enter 34
Second Input: Enter 56
Operation: Select - (subtraction)
Result: Display shows Result: -22

✨ Features

🎨 Graphical User Interface - Clean and intuitive dialog-based interface using Zenity
➕ Basic Arithmetic Operations - Addition, Subtraction, Multiplication, and Division
🔢 Decimal Support - Handles both integers and floating-point numbers with high precision (up to 10 decimal places)
⚠️ Error Handling - Validates division by zero and invalid operations
❌ Graceful Exit - User can cancel at any step without errors
🚀 Lightweight - Minimal dependencies, fast execution
📊 Precision Calculations - Uses GNU bc for accurate arithmetic

