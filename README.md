This is a simple HTML form with client-side validation using JavaScript. The form is styled using Bootstrap 5. The form collects basic user information like name, email, phone number, and password, and it validates the inputs before submission.

Features
.Uses Bootstrap 5 for styling.
.Includes client-side validation to ensure the user provides a valid name, email, phone number, and password.
.Provides real-time validation feedback to the user through alerts and prevents submission of invalid data.

Form Structure
The form includes the following fields:

.Name (text input)
.Email (email input)
.Phone Number (telephone input)
.Password (password input)

![FormValidationpic](https://github.com/user-attachments/assets/8e7c343a-0789-4717-aab2-98ea06bfec24)

JavaScript Validation Logic
The validation logic ensures that:
.Name: Must not be empty and should not contain numbers.
.Email: Must not be empty (you can extend this with regex for a valid email format).
.Phone Number: Must be 10 digits long.
.Password: Must not be empty and should be at least 5 characters long.

The validation occurs when the user submits the form. If any field fails the validation, the form submission is prevented, and an alert is shown to the user.

How it Works:
1.When the form is submitted, the submit event listener runs.
2.Each input is checked for validity:
    .Empty inputs show an alert.
    .For the name, it checks if the input contains only letters.
    .The phone number must have exactly 10 digits.
    .The password must have a minimum length of 5 characters.
3.If any validation fails, the form submission is prevented, and the corresponding alert is shown.
