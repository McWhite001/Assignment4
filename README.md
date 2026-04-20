# Assignment4
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Registration Form</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            max-width: 600px;
            margin: 50px auto;
            padding: 20px;
            background-color: #f5f5f5;
        }
        form {
            background-color: white;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        h1 {
            text-align: center;
            color: #333;
            margin-bottom: 30px;
        }
        .form-group {
            margin-bottom: 20px;
        }
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
            color: #555;
        }
        input[type="text"],
        input[type="number"],
        input[type="email"],
        input[type="tel"],
        input[type="password"] {
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 4px;
            box-sizing: border-box;
            font-size: 14px;
        }
        .radio-group,
        .checkbox-group {
            display: flex;
            flex-direction: column;
            gap: 8px;
        }
        .radio-group label,
        .checkbox-group label {
            font-weight: normal;
            display: flex;
            align-items: center;
            gap: 8px;
            cursor: pointer;
        }
        .radio-group input,
        .checkbox-group input {
            width: auto;
            cursor: pointer;
        }
        .button-group {
            display: flex;
            gap: 10px;
            margin-top: 30px;
        }
        button {
            flex: 1;
            padding: 12px;
            border: none;
            border-radius: 4px;
            font-size: 16px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        button[type="submit"] {
            background-color: #4CAF50;
            color: white;
        }
        button[type="submit"]:hover {
            background-color: #45a049;
        }
        button[type="reset"] {
            background-color: #f44336;
            color: white;
        }
        button[type="reset"]:hover {
            background-color: #da190b;
        }
    </style>
</head>
<body>

    <form action="#" method="post">
        <h1>Student Registration Form</h1>

        <!-- Q2: Text inputs with labels -->
        <div class="form-group">
            <label for="firstName">First Name</label>
            <input type="text" id="firstName" name="firstName" placeholder="Enter your first name" required>
        </div>

        <div class="form-group">
            <label for="lastName">Last Name</label>
            <input type="text" id="lastName" name="lastName" placeholder="Enter your last name" required>
        </div>

        <!-- Q3: Number input -->
        <div class="form-group">
            <label for="age">Age</label>
            <input type="number" id="age" name="age" min="10" max="99" placeholder="Enter your age (10-99)" required>
        </div>

        <!-- Q4: Email input -->
        <div class="form-group">
            <label for="email">Email Address</label>
            <input type="email" id="email" name="email" placeholder="example@email.com" required>
        </div>

        <!-- Q5: Telephone input -->
        <div class="form-group">
            <label for="phone">Phone Number</label>
            <input type="tel" id="phone" name="phone" placeholder="+234 800 000 0000">
        </div>

        <!-- Q6: Password input -->
        <div class="form-group">
            <label for="password">Password</label>
            <input type="password" id="password" name="password" minlength="8" placeholder="Minimum 8 characters" required>
        </div>

        <!-- Q7: Radio buttons — gender -->
        <div class="form-group">
            <label>Gender</label>
            <div class="radio-group">
                <label for="male">
                    <input type="radio" id="male" name="gender" value="male" required>
                    Male
                </label>
                <label for="female">
                    <input type="radio" id="female" name="gender" value="female">
                    Female
                </label>
                <label for="preferNotToSay">
                    <input type="radio" id="preferNotToSay" name="gender" value="preferNotToSay">
                    Prefer not to say
                </label>
            </div>
        </div>

        <!-- Q8: Checkboxes — courses -->
        <div class="form-group">
            <label>Courses Interested In</label>
            <div class="checkbox-group">
                <label for="webDev">
                    <input type="checkbox" id="webDev" name="courses" value="webDevelopment">
                    Web Development
                </label>
                <label for="dataScience">
                    <input type="checkbox" id="dataScience" name="courses" value="dataScience">
                    Data Science
                </label>
                <label for="mobileDev">
                    <input type="checkbox" id="mobileDev" name="courses" value="mobileDevelopment">
                    Mobile App Development
                </label>
                <label for="cyberSec">
                    <input type="checkbox" id="cyberSec" name="courses" value="cyberSecurity">
                    Cyber Security
                </label>
                <label for="ai">
                    <input type="checkbox" id="ai" name="courses" value="artificialIntelligence">
                    Artificial Intelligence
                </label>
            </div>
        </div>

        <!-- Q9: Submit and reset buttons -->
        <div class="button-group">
            <button type="submit">Register Now</button>
            <button type="reset">Clear Form</button>
        </div>

    </form>

    <!-- 
        Q10 BONUS: Reflection
        A radio button allows only one selection from a group of options (single choice), 
        while a checkbox allows multiple selections independently (multiple choices).
    -->

</body>
</html>
