# Radio State Calculator


An arithmetic calculation engine that evaluates addition directly within the rendering pipeline using pure selector combinators and counters.

## Overview

This project demonstrates declarative state evaluation. By binding DOM form controls directly to layout styling rules, two separate numeric inputs are captured, parsed, and combined inside the layout calculation stage. It removes execution scripting entirely while preserving dynamic user interactions.

## How It Works

1. **State Persistence:** Hidden HTML radio inputs track user selections for two distinct operands (`num1` and `num2`).
2. **Selector Cascading:** Subsequent sibling combinators (`~`) detect active inputs and target the display element.
3. **Evaluation Rules:** Specific style declarations increment counter variables using predefined addition lookup logic.
4. **Output Rendering:** The computed output displays dynamically using pseudo-element content binding.

## Key Features

* **Zero Execution Engine:** Operates without relying on script runtime contexts.
* **Deterministic Evaluation:** Implements explicit combination matrices for instantaneous feedback.
* **Native Reset Handling:** Built-in form reset behavior restores baseline state across controls.

## Tech Stack Breakdown

* **HTML5:** Semantic form markup utilizing `<input type="radio">` and associated `<label>` controls.
* **CSS3:** Advanced usage of general sibling combinators (`~`), custom variables, and counter functions (`counter-reset`, `counter()`).

## Prerequisites & Web-Based Quick Start

You do not need a terminal or a local development environment.

### Quick Start via GitHub Codespaces

1. Click the **Code** button at the top right of this repository.
2. Select the **Codespaces** tab and click **Create codespace on main**.
3. Open `index.html` inside your browser preview within the web editor.

### Manual Web Setup

1. Download the repository source directly from the browser as a ZIP file.
2. Extract the archive on your local system.
3. Double-click `index.html` to open it in any web browser.

## Project Structure

```text
radio-state-calculator/
├── .github/
│   └── workflows/
│       └── validate-markup.yml  # Automated markup validation workflow
├── .gitignore                    # Local environment exclusion file
├── index.html                    # Application interface and input structure
├── style.css                     # Combinator evaluation matrix and rules
└── LICENSE                       # MIT open source license
```

## Roadmap

[ ] Expand combination matrix to cover subtraction operations.

[ ] Implement multi-digit value selectors up to 10.

[ ] Add visual state indicators for selected operands.

```text
"Constraint drives engineering creativity."
```
