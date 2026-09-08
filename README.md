# Web Terminal Simulator

An interactive and highly customizable web terminal simulator, built entirely in a single file using HTML, CSS, and Vanilla JavaScript. This project emulates the look and feel of a classic macOS/Linux terminal, featuring a virtual file system, a simulated package manager, and dynamic UI layout commands.

---

## Main Features

* **Classic Interface:** Retro design with a solid dark background, monospace font, and dynamic text output.
* **Virtual File System:** Seamless navigation through simulated folders and files using a JSON structure.
* **Dynamic Status Bar:** Displays the current directory (`pwd`) and can be moved around the screen or hidden.
* **Simulated Package Manager (`apt`):** Allows users to "install" tools with realistic loading animations and simulated network delays.
* **Fake Nmap Scanner:** A highly realistic port scanning simulation, designed exclusively for testing and demonstration purposes.
* **Zero Dependencies:** All code (UI layout, styling, and logic) lives inside a single `index.html` file.

---

## Available Commands

### Standard Commands (Linux / macOS)
* `ls` : Lists the contents of the current directory (folders are highlighted in a different color).
* `cd [directory]` : Changes the current working directory.
* `pwd` : Displays the full path of the current working directory.
* `echo [text]` : Prints the entered text to the screen.
* `clear` : Clears the terminal history.
* `whoami` : Displays the current user's name.
* `date` : Displays the system date and time.

### Customization Commands
* `color [text] [background]` : Changes the terminal colors in real-time (e.g., `color #00ff00 black`).
* `turn [position]` : Moves the status bar. Options include: `top`, `down`, `left`, `off` (hide), and `on` (show).

### Package Manager (Simulation)
* `apt list` : Displays a cleanly formatted list of all available packages and their current status (Installed / Available).
* `apt install [package]` : Initiates the simulated installation sequence for a given package.
* `nmap -p- -sV <IP>` : (Requires prior installation via `apt`) Executes a mock network scan displaying fake open ports and services.

---

## Getting Started

Installation is immediate, as it requires no backend servers or databases.

1. Download or clone this repository.
2. Double-click the `index.html` file to open it in any modern web browser (Chrome, Firefox, Safari, Edge).
3. Start typing commands!

---

## Technologies Used

* **HTML5:** Semantic UI structure.
* **CSS3:** Flexbox/Grid for dynamic layout management and CSS Variables for real-time color switching.
* **Vanilla JavaScript (ES6+):** File system logic, DOM manipulation, promises (`async/await`) for realistic time delays, and command routing.
