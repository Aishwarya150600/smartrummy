<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Wow Rummy Club Login</title>
</head>
<body>
   <div class="container">
        <div class="logo">
            <h1>SMART RUMMY CLUB</h1>
        </div>
        <div class="form-container">
            <h2>Welcome! Log in & start WINNING!</h2>
            <form id="loginForm">
                <input type="text" id="username" placeholder="Phone Number or Email" required>
                <input type="password" id="password" placeholder="Password" required>
                <a href="#" class="forgot-password">Forgot Password?</a>
            </form>
        </div>
    </div>
    <script src="script.js"></script>

<div id="loginScreen">
    <button id="loginButton">Login</button>
    </form>
            <p>New to Smart Rummy Club? <a href="#" class="join-now">Join Now</a></p>
            <button class="guest-login">Guest Login</button>
</div>

<div id="secondScreen" style="display: none;">
    <h1>Game Room</h1>
    <div class="game-menu">
        <!-- Your second image content goes here -->
        <h2>User: USER_44159952</h2>
        <span>Cash: ₹0.00</span>
        <button>Add Cash</button>
        <div>
            <label>Select Players:</label>
            <input type="radio" name="players" value="2"> 2 Players
            <input type="radio" name="players" value="6"> 6 Players
        </div>
        <div>
            <label>Entry Fee:</label>
            <input type="range" min="0.01" max="200" step="0.01" value="0.01" id="entryFeeRange">
            <span id="entryFeeDisplay">₹0.01</span>
        </div>
        <button>Play Now</button>
    </div>
</div>

<script src="script.js"></script>
</body>
</html>

body {
    font-family: Arial, sans-serif;
    background-color: #521c21; /* Dark red background */
    color: white; /* White text color */
    text-align: center;
}

.game-menu {
    background-color: #70333c; /* Lighter red for game menu */
    padding: 20px;
    border-radius: 10px;
    display: inline-block;
}

button {
    background-color: #c8b461; /* Gold buttons */
    color: black;
    border: none;
    padding: 10px 20px;
    cursor: pointer;
    border-radius: 5px;
    margin: 10px;
}


document.getElementById('loginButton').addEventListener('click', function() {
    document.getElementById('loginScreen').style.display = 'none';
    document.getElementById('secondScreen').style.display = 'block';
});

document.getElementById('entryFeeRange').addEventListener('input', function() {
    document.getElementById('entryFeeDisplay').innerText = `₹${this.value}`;
});
