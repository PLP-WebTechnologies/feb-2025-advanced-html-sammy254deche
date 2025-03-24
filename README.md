# Advanced HTML5 Elements and Forms

## Objectives
Implement HTML5 images, lists, tables, forms and input types.
Use form validation attributes.
Apply multimedia elements such as audio and video.

## Instructions

- Create an index.html file.
- Add an ordered list with roman numerals
- Add an external image from pexels.com
- Add a table of 5 contacts with; name, address, mobile and emails
- Add a registration form

>[!NOTE]
>  The registration form should have:
>- Name, email, password, and date fields.
>- A dropdown, radio buttons, and checkboxes.
>- Proper labels and placeholders.
>- Required fields and validation attributes.
>- Ensure proper indentation and commenting.
 
# Tasks
- Create a well-structured HTML5 document.
- Ensure semantic correctness.

Happy Coding! 💻✨



```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML5 Document</title>
    <!-- External stylesheet or internal CSS can be linked here -->
</head>
<body>
    <!-- Ordered List with Roman Numerals -->
    <section>
        <h2>Ordered List</h2>
        <ol type="I">
            <li>First Item</li>
            <li>Second Item</li>
            <li>Third Item</li>
        </ol>
    </section>

    <!-- External Image -->
    <section>
        <h2>Image</h2>
        <img src="https://images.pexels.com/photos/1234567/example.jpg" alt="Descriptive Image Alt Text" style="max-width:100%; height:auto;">
        <!-- Replace the image URL with an actual one from Pexels -->
    </section>

    <!-- Table of Contacts -->
    <section>
        <h2>Contacts</h2>
        <table border="1" cellpadding="5" cellspacing="0">
            <thead>
                <tr>
                    <th>Name</th>
                    <th>Address</th>
                    <th>Mobile</th>
                    <th>Email</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>John Doe</td>
                    <td>123 Main St</td>
                    <td>+1234567890</td>
                    <td>johndoe@example.com</td>
                </tr>
                <tr>
                    <td>Jane Smith</td>
                    <td>456 Elm St</td>
                    <td>+1987654321</td>
                    <td>janesmith@example.com</td>
                </tr>
                <tr>
                    <td>Bob Johnson</td>
                    <td>789 Pine St</td>
                    <td>+1122334455</td>
                    <td>bobjohnson@example.com</td>
                </tr>
                <tr>
                    <td>Alice Brown</td>
                    <td>101 Maple St</td>
                    <td>+2233445566</td>
                    <td>alicebrown@example.com</td>
                </tr>
                <tr>
                    <td>Charlie White</td>
                    <td>202 Oak St</td>
                    <td>+3344556677</td>
                    <td>charliewhite@example.com</td>
                </tr>
            </tbody>
        </table>
    </section>

    <!-- Registration Form -->
    <section>
        <h2>Registration Form</h2>
        <form action="#" method="post">
            <!-- Name Field -->
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" placeholder="Enter your name" required><br>

            <!-- Email Field -->
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" placeholder="Enter your email" required><br>

            <!-- Password Field -->
            <label for="password">Password:</label>
            <input type="password" id="password" name="password" placeholder="Enter your password" required minlength="8"><br>

            <!-- Date Field -->
            <label for="date">Date of Birth:</label>
            <input type="date" id="date" name="date" required><br>

            <!-- Dropdown -->
            <label for="country">Country:</label>
            <select id="country" name="country" required>
                <option value="">Select your country</option>
                <option value="Kenya">Kenya</option>
                <option value="Uganda">Uganda</option>
                <option value="Tanzania">Tanzania</option>
            </select><br>

            <!-- Radio Buttons -->
            <p>Gender:</p>
            <label><input type="radio" name="gender" value="male" required> Male</label>
            <label><input type="radio" name="gender" value="female"> Female</label>
            <label><input type="radio" name="gender" value="other"> Other</label><br>

            <!-- Checkboxes -->
            <p>Interests:</p>
            <label><input type="checkbox" name="interests" value="sports"> Sports</label>
            <label><input type="checkbox" name="interests" value="music"> Music</label>
            <label><input type="checkbox" name="interests" value="reading"> Reading</label><br>

            <!-- Submit Button -->
            <button type="submit">Register</button>
        </form>
    </section>
</body>
</html>
```
