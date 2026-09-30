# Python Bistro

A menu-driven command-line restaurant ordering and billing system developed in Python.

## Project Information

| Field | Details |
|---|---|
| **Project Title** | Python Bistro |
| **Student Name** | Alan S Kumar |
| **Registration Number** | 26BCE10296 |
| **Language** | Python 3 |
| **Application Type** | Command-Line Application |
| **External Libraries** | None required |

## Overview

**Python Bistro** is a simple restaurant ordering and billing application. It allows a customer to enter their name, select an order type, choose food items and quantities from a predefined menu, review the current order, and generate a final bill.

The application demonstrates core Python programming and problem-solving concepts including functions, dictionaries, loops, conditional statements, input validation, exception handling, modular programming, and automated testing.

## Features

- Accepts and validates the customer's name.
- Supports **Dine-In** and **Takeaway** orders.
- Displays a predefined menu containing 10 food and beverage items.
- Allows multiple items and quantities to be added to an order.
- Combines quantities when the same item is selected more than once.
- Displays the current order and subtotal.
- Automatically calculates **5% GST**.
- Generates a formatted final bill.
- Handles invalid menu choices and non-numeric input.
- Includes a separate test module for billing calculations.

## Menu

| No. | Item | Price (INR) |
|---:|---|---:|
| 1 | Burger | 120 |
| 2 | Pizza | 180 |
| 3 | Pasta | 150 |
| 4 | French Fries | 80 |
| 5 | Sandwich | 100 |
| 6 | Cold Coffee | 70 |
| 7 | Coke | 50 |
| 8 | Coffee | 25 |
| 9 | Tea | 20 |
| 10 | Thali | 180 |

GST is calculated at **5%** on the subtotal.

## Project Structure

```text
PythonBistro/
│
├── main.py
├── utils.py
├── test_bistro.py
├── statement.md
├── README.md
│
└── docs/
    ├── flowchart.png
    ├── use_case_diagram.png
    ├── sequence_diagram.png
    ├── system_architecture.png
    ├── component_diagram.png
    ├── requirements.png
    ├── objectives.png
    ├── sample_output.png
    ├── test_results.png
    ├── test_results.txt
    └── Python_Bistro_Project_Report.pdf
```

## File Description

### `main.py`
Contains the main application flow. It handles:
- Customer input
- Order type selection
- Menu interaction
- Order management
- Bill generation
- Input validation

### `utils.py`
Contains reusable data and calculation functions:
- Menu data
- GST rate
- Subtotal calculation
- GST calculation
- Final total calculation
- Menu printing
- Bill printing

### `test_bistro.py`
Contains tests for:
- Single-item calculations
- Multiple-item calculations
- GST calculation
- Final bill calculation
- Empty orders
- A complete bill calculation

### `statement.md`
Contains the problem statement, objectives, functional modules, non-functional requirements, and project scope.

### `docs/`
Contains design diagrams, requirements/objectives documentation, sample output, and test evidence.

## Requirements

- Python 3.x
- No external packages are required.

## How to Run

Open a terminal in the project folder and run:

```bash
python main.py
```

Follow the on-screen menu to place an order and generate the bill.

## How to Test

Run:

```bash
python test_bistro.py
```

Expected output:

```text
ALL TESTS PASSED!
```

The included test suite currently passes all six test cases.

## Billing Logic

The application uses the following formulas:

```text
Subtotal = Σ (Item Price × Quantity)

GST = Subtotal × 0.05

Final Bill = Subtotal + GST
```

For example, if the subtotal is INR 1000:

```text
GST = 1000 × 0.05 = INR 50
Final Bill = 1000 + 50 = INR 1050
```

## Input Validation

The program validates:
- Empty customer names
- Non-numeric menu choices
- Invalid menu item numbers
- Invalid order-type choices
- Quantities less than or equal to zero

Invalid input does not terminate the program; the user is prompted to enter a valid value.

## Design Documentation

The `docs` folder contains:
- System requirements
- Project objectives
- Flowchart
- Use case diagram
- Sequence diagram
- System architecture
- Component diagram
- Sample execution output
- Test results
- Complete project report

## Limitations

- Data is stored only in memory while the program is running.
- There is no database or persistent storage.
- The application is command-line based.
- There is no online payment functionality.
- There is no user account or authentication system.
- Menu data is predefined in the source code.

## Future Enhancements

Possible extensions include:
- Persistent order storage
- Customer order history
- Table-number management
- Discounts and coupons
- Multiple GST/tax categories
- Receipt export to PDF
- Database integration
- Graphical user interface
- Online ordering and payment
- Admin menu management

## Author

**Alan S Kumar**  
**Registration Number: 26BCE10296**

## Academic Note

This project is intended as a Python programming/problem-solving project demonstrating modular programming, input handling, calculations, and testing through a practical restaurant billing use case.
