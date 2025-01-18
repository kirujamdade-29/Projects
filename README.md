Age Calculator Web Application

Welcome to the Age Calculator web application! This project is a simple, interactive tool for calculating your exact age in terms of years, months, and days.
Features
Responsive Design: The application adjusts beautifully across devices thanks to its CSS styling.
Dynamic Date Validation: Prevents selecting a future date using JavaScript.
Detailed Results: Displays your exact age in years, months, and days with a user-friendly UI.
Stylish UI: A gradient background, modern font, and interactive buttons enhance the user experience.

Files in This Project
1. index.html
The HTML file provides the structure of the application. Key components include:
Container for the Calculator: Includes a title, input field for the date, and a button to calculate the age.
Result Display Area: Dynamically shows the calculated age.

Code Highlights:
Date Input Restriction:

let userInput = document.getElementById("date");
userInput.max = new Date().toISOString().split("T")[0];

This ensures users cannot select a date in the future.

Age Calculation Logic:

function calculateAge() {
    let birthDate = new Date(userInput.value);
    // Detailed logic for calculating age in years, months, and days.
    result.innerHTML = `You are <span>${y3}</span> years, <span>${m3}</span> months, and <span>${d3}</span> days old`;
}

Utility Function:

function getDaysInMonth(year, month) {
    return new Date(year, month, 0).getDate();
}

This function dynamically determines the number of days in a month, accounting for leap years.

2. style.css
The CSS file styles the application, making it visually appealing.

Key Styling Elements:

Background:

.container {
    background: linear-gradient(135deg, #4203a9, #90bafc);
}

A gradient background provides a modern look.

Calculator Box:

.Calculator {
    max-width: 600px;
    margin-top: 10%;
    margin-left: 10%;
}

Centers and sizes the calculator for a professional appearance.

Interactive Elements:

Buttons have hover effects and clear visual feedback.

The date picker input is styled for better usability.

How to Use

Open the index.html file in your web browser.

Select your birthdate using the date picker.

Click the "Calculate" button.

View your age in the results area.

Requirements

A modern web browser (Chrome, Firefox, Edge, etc.).

No external dependencies; everything is handled within the two provided files.

Customization

You can modify the following:

Background Colors: Edit the gradient in the .container class in style.css.

Font Style: Replace 'Poppins' with your preferred font in style.css.

Button Styles: Customize the colors, padding, or hover effects in the .input-box button class.

Future Enhancements

Add time calculations for hours, minutes, and seconds.

Include additional validations for edge cases.

Expand the application to support multiple languages.

Acknowledgments

Font: Uses the Poppins font for a clean and modern look.

Gradient Inspiration: Derived from popular UI design trends.

Enjoy calculating your age with this simple and intuitive tool!
