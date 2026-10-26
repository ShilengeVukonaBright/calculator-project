# CALCULATE – Simple Web Calculator

A lightweight, browser-based calculator built with HTML, CSS, and JavaScript. It handles basic arithmetic and runs with no installation, no frameworks, and no build step.

## Features

- Addition (`+`), subtraction (`-`), multiplication (`*`), and division (`/`)
- Decimal number support (`.`)
- Clear button (`C`) to reset the display
- Right-aligned, read-only display so users can't type invalid characters
- Shows `Error` when an expression is invalid
- Colour-coded buttons: operators in blue, equals in green, clear in red
- Hover effect on buttons for visual feedback
- Responsive viewport setup for mobile and desktop screens

## Built With

- **HTML5**: structure of the calculator
- **CSS3**: layout (CSS Grid and Flexbox) and styling
- **JavaScript (vanilla)**: calculator logic
- **Google Fonts**: [Poppins](https://fonts.google.com/specimen/Poppins)

## Project Structure

```
calculator/
├── index.html    # Page structure and buttons
├── style.css     # Styling and layout
├── main.js       # Calculator logic
└── README.md
```

> If your HTML file has a different name, update it here.

## Getting Started

### Prerequisites

- Any modern web browser (Chrome, Firefox, Edge, Safari)
- Internet connection for the Poppins font (the calculator still works without it, using the fallback `sans-serif` font)

### Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/your-repo.git
   ```
2. Open the project folder:
   ```bash
   cd your-repo
   ```
3. Open `index.html` in your browser (double-click it, or right-click and choose **Open with** your browser).

## How to Use

1. Click the number buttons to enter your first number.
2. Click an operator (`+`, `-`, `*`, `/`).
3. Enter the second number.
4. Click `=` to see the result.
5. Click `C` to clear the display and start again.

## How It Works

- `appendToDisplay(input)` adds the clicked button's value to the display.
- `clearDisplay()` empties the display.
- `calculate()` evaluates the expression on the display and shows the result. If the expression is invalid, the display shows `Error`.

## Known Limitations

- No keyboard input yet (buttons only)
- No delete/backspace button, only full clear
- The calculation uses JavaScript's `eval()`. This is fine for a small learning project where input comes only from the buttons, but it should be replaced with a safer expression parser if the calculator is ever extended to accept typed input.
- Operator buttons use `*` and `/` rather than `×` and `÷`

## Future Improvements

- Keyboard support
- Backspace button
- Replace `eval()` with a safe parsing function
- Percentage and square root functions
- Calculation history
- Dark mode

## Author

https://github.com/ShilengeVukonaBright
