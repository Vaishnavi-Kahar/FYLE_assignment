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

### 1. Age Group Selection

The age dropdown field requires users to select one of the three provided options: <40, ≥ 40 & < 60, or ≥ 60.

![Age group Screenshot](/screenshots/ageGroup.png)

### 2. Tax Calculation for Income Less than 8 Lakhs (No Tax Deducted)

When the total income (after deductions) is less than 8 Lakhs, no tax is deducted. The app correctly handles this scenario and displays a message indicating that no tax is deducted. Below is a screenshot of this scenario:

![No Tax Deducted Screenshot](/screenshots/noTax1.png)
![No Tax Deducted Screenshot](/screenshots/noTax2.png)

### 3. Tax Calculation for Income Exceeding 8 Lakhs

When the total income (after deductions) exceeds 8 Lakhs, the app correctly calculates the tax amount based on the user's age group and income level. The tax amount is deducted from the total income, and the remaining income after tax deduction is displayed on a modal. Below is a screenshot of this scenario:

![Tax Calculation Exceeding 8 Lakhs Screenshot](/screenshots/Tax1.png)
![Tax Calculation Exceeding 8 Lakhs Screenshot](/screenshots/Tax2.png)


### 4. Handling Invalid Fields

The app validates input fields to ensure that only numeric values are entered in number fields. If a user enters invalid input, error icons are displayed below the respective input fields, indicating the error. Below is a screenshot illustrating this scenario:

![Invalid Fields Screenshot](/screenshots/invalid.png)

### 5. Handling Required Inputs

The app ensures that all mandatory fields, such as the age group selection, are filled before submission. If a user attempts to submit the form without filling out required fields, a message is displayed prompting the user to fill the missing fields. Below is a screenshot depicting this scenario:

![Required Inputs Missing Screenshot](/screenshots/mandatory.png)

### 6. What each field is about

The app has question-mark icon next to each field title which diplays what that field is about when clicked on, and stays for 3 seconds.

![Question Screenshot](/screenshots/question.png)

## Installation Instructions

1. Clone the repository: `git clone https://github.com/Vaishnavi-Kahar/FYLE_assignment.git`
2. Navigate to the project directory.
3. Open `index.html` in a web browser.

## Live Demo

Live demo is availbale [here](https://vaishnavi-kahar.github.io/FYLE_assignment/)



By Vaishnavi Kahar

