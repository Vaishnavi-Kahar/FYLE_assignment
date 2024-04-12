# Tax Calculator App

## Overview

The Tax Calculator App is a web-based application designed to help users calculate their income tax based on their gross annual income, extra income, age group, and applicable deductions. The app follows specific tax calculation formulas based on the user's age and total income. It provides real-time error validation to ensure accurate input and displays the calculated tax amount in a modal dialog.

## Technologies Used

- HTML
- CSS
- JavaScript
- Bootstrap 4

## References & Requirements

### Tax Calculation Formula

- Overall income (after deductions) under 8 (≤) Lakhs is not taxed.
- Income over 8 (>) Lakhs is taxed based on the following rates:
  - 30% for people with age < 40
  - 40% for people with age ≥ 40 but < 60
  - 10% for people with age ≥ 60

### Requirements

- Allow users to input gross annual income, extra income, age group, and deductions.
- Highlight error icons for incorrect values in number fields and show tooltips when clicked.
- Age dropdown field must have three values: <40, ≥ 40 & < 60, and ≥ 60.
- Display error icons and tooltips for mandatory input fields if user attempts to submit without entering values.
- Modal should display the calculated tax amount and income after deductions upon submission.

## Example

Suppose a user, aged 34, has a gross annual income of 40 Lakhs with no deductions. The tax calculation would be: 30% * (40 - 8) = 9.6 Lakhs.

## Edge Cases Covered

### 1. Non-Numeric Input Handling

To prevent users from entering non-numeric values in number fields, the app employs client-side validation. Error icons are displayed with a message below the input fields, indicating invalid input. 

### 2. Age Group Selection

The age dropdown field requires users to select one of the three provided options: <40, ≥ 40 & < 60, or ≥ 60. If a user attempts to submit the form without selecting an age group, an error icon appears next to the dropdown field, indicating that the input is mandatory.

### 3. Income Exceeding 8 Lakhs

When the total income (after deductions) exceeds 8 Lakhs, the app correctly calculates the tax amount based on the user's age group and income level. The tax rates are applied as per the specified formula, ensuring accurate tax calculation for different age groups.

## Installation Instructions

1. Clone the repository: `git clone https://github.com/Vaishnavi-Kahar/FYLE_assignment.git`
2. Navigate to the project directory.
3. Open `index.html` in a web browser.

## Live Demo

[https://vaishnavi-kahar.github.io/FYLE_assignment/]



- Vaishnavi Kahar

