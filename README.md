# OmniCLI

OmniCLI is a lightweight, all-in-one terminal application built in C++. It provides a collection of essential tools and classic games within a single interactive environment, designed for users who prefer staying in the command line.

The application uses `termios` to handle raw keyboard input, allowing for smooth, real-time navigation without needing to press "Enter" for every selection.

## Features

The suite includes eight distinct modules:

* **Calculator:** Perform basic arithmetic (+, -, *, /).
* **PhoneBook:** Save and view contact names and numbers.
* **MemoPad:** A text editor to write and save quick notes.
* **Address Book:** Manage detailed addresses (Street, City, Zip).
* **Sudoku:** A playable 9x9 Sudoku puzzle with random board generation.
* **Calendar:** A month-by-month viewer with easy navigation.
* **Wallpaper:** Switch between different ASCII art branding styles.
* **Tic-Tac-Toe:** Play a match against a computer opponent.

## Controls

Navigation uses a standard "WASD" layout for terminal movement:

| Key | Action |
| :--- | :--- |
| **W** | Move selection Up |
| **S** | Move selection Down |
| **A** | Move selection Left |
| **D** | Move selection Right |
| **X** | Select / Open a module |
| **B** | Go back to the previous menu |
| **Q** | Quit (in specific modules) |



## Technical Details

* **Language:** C++
* **Input Handling:** Custom `getch()` implementation using `termios.h`.
* **Persistence:** Saves data to local `.txt` files (`memo.txt`, `contacts.txt`, `addresses.txt`).
* **Compatibility:** Designed for Unix-like environments (Linux/macOS).

## Getting Started

### Prerequisites
You will need a C++ compiler (like `g++`) installed on your system.

### Installation
1. Clone the repository:
    ```bash
    git clone [https://github.com/yourusername/omniscli.git](https://github.com/yourusername/omnicli.git)
    cd omnicli
    ```
    
2. Compile the source code:
    ```
    g++ -o omnicli main.cpp
    ```
    
Run the application:
    ```
    ./omnicli
    ```
