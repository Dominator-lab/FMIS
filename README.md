<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Website with Sign-In/Sign-Up</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Welcome to My Website</h1>
    </header>

    <main>
        <p>Sign in or sign up to access exclusive content!</p>
        <button onclick="showModal('signin')">Sign In</button>
        <button onclick="showModal('signup')">Sign Up</button>
    </main>

    <!-- Sign In Modal -->
    <div id="signinModal" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closeModal('signinModal')">&times;</span>
            <h2>Sign In</h2>
            <form id="signinForm" onsubmit="handleSignIn(event)">
                <label for="signinEmail">Email:</label>
                <input type="email" id="signinEmail" required>
                <label for="signinPassword">Password:</label>
                <input type="password" id="signinPassword" required>
                <button type="submit">Sign In</button>
            </form>
        </div>
    </div>

    <!-- Sign Up Modal -->
    <div id="signupModal" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closeModal('signupModal')">&times;</span>
            <h2>Sign Up</h2>
            <form id="signupForm" onsubmit="handleSignUp(event)">
                <label for="signupEmail">Email:</label>
                <input type="email" id="signupEmail" required>
                <label for="signupPassword">Password:</label>
                <input type="password" id="signupPassword" required>
                <button type="submit">Sign Up</button>
            </form>
        </div>
    </div>

    <footer>
        <p>&copy; 2024 Simple Website</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
