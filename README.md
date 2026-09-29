<!doctype html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Maggi Corner</title>
<style>
/* General Styling */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
}


/* Header */

header {
    background-color: #e63900;
    color: white;
    text-align: center;
    padding: 25px;
}

header h1 {
    font-size: 35px;
}

header p {
    font-size: 18px;
}


/* Navigation */

nav {
    background-color: #222;
    text-align: center;
    padding: 15px;
}

nav a {
    color: white;
    text-decoration: none;
    margin: 0 20px;
    font-size: 17px;
}

nav a:hover {
    color: #ffcc00;
}


/* Hero Section */

.hero {
    height: 400px;

    background-image: url("https://images.unsplash.com/photo-1569718212165-3a8278d5f624");

    background-size: cover;
    background-position: center;

    display: flex;
    justify-content: center;
    align-items: center;

    text-align: center;
}

.hero-content {
    background-color: rgba(0, 0, 0, 0.7);
    color: white;

    padding: 40px;
    border-radius: 10px;
}

.hero-content h2 {
    font-size: 40px;
}

.hero-content p {
    font-size: 18px;
    margin: 15px 0;
}


/* Buttons */

button {
    background-color: #ffb300;
    color: #222;

    border: none;
    padding: 12px 25px;

    font-size: 16px;
    font-weight: bold;

    border-radius: 5px;

    cursor: pointer;
}

button:hover {
    background-color: #ff8c00;
}


/* About Section */

.about {
    text-align: center;
    padding: 50px 15%;
}

.about h2 {
    margin-bottom: 20px;
    font-size: 30px;
}


/* Menu Section */

#menu {
    background-color: #fff4d6;

    padding: 50px;

    text-align: center;
}

#menu h2 {
    font-size: 30px;

    margin-bottom: 30px;
}


/* Food Cards */

.menu-container {
    display: flex;

    justify-content: center;

    gap: 25px;

    flex-wrap: wrap;
}

.food-card {
    background-color: white;

    width: 250px;

    padding: 15px;

    border-radius: 10px;

    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);

    transition: 0.3s;
}

.food-card:hover {
    transform: translateY(-8px);
}

.food-card img {
    width: 100%;

    height: 170px;

    object-fit: cover;

    border-radius: 8px;
}

.food-card h3 {
    margin: 10px 0;
}

.food-card h4 {
    font-size: 20px;

    margin: 10px;
}


/* Offers */

.offers {
    text-align: center;

    padding: 50px;
}

.offers h2 {
    margin-bottom: 25px;
}

.offer-box {
    background-color: #e63900;

    color: white;

    max-width: 500px;

    margin: auto;

    padding: 30px;

    border-radius: 10px;
}

.offer-box h3 {
    font-size: 25px;

    margin-bottom: 10px;
}


/* Contact */

.contact {
    background-color: #f5f5f5;

    text-align: center;

    padding: 50px;
}

.contact h2 {
    margin-bottom: 20px;
}


/* Footer */

footer {
    background-color: #222;

    color: white;

    text-align: center;

    padding: 20px;
}
/* Order Popup */

.modal,
.success {
    display: none;

    position: fixed;

    z-index: 1000;

    left: 0;
    top: 0;

    width: 100%;
    height: 100%;

    background: rgba(0, 0, 0, 0.7);

    justify-content: center;
    align-items: center;

    padding: 20px;
}

.order-box,
.success-box {
    background: white;

    width: 100%;
    max-width: 450px;

    padding: 30px;

    border-radius: 10px;

    position: relative;
}

.order-box h2,
.success-box h2 {
    text-align: center;
    margin-bottom: 20px;
}

.close {
    position: absolute;

    right: 15px;
    top: 5px;

    font-size: 30px;

    cursor: pointer;
}

.order-box label {
    display: block;

    margin-top: 10px;

    font-weight: bold;
}

.order-box input,
.order-box textarea {
    width: 100%;

    padding: 10px;

    margin-top: 5px;

    border: 1px solid #ccc;

    border-radius: 5px;
}

.order-box textarea {
    height: 70px;
}

.order-box form button {
    width: 100%;
    margin-top: 15px;
}

.order-box h3 {
    text-align: center;

    margin-top: 15px;

    color: #e63900;
}

.success-box {
    text-align: center;
}

.success-box button {
    margin-top: 15px;
}
</style>
    <link rel="stylesheet" href="style.css">
</head>

<body>

    <!-- Header -->
    <header>
        <h1>Maggi Corner</h1>
        <p>Hot, Tasty & Delicious Maggi</p>
    </header>


    <!-- Navigation -->
    <nav>
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#menu">Menu</a>
        <a href="#offers">Offers</a>
        <a href="#contact">Contact</a>
    </nav>


    <!-- Home Section -->
    <section id="home" class="hero">

        <div class="hero-content">

            <h2>Welcome to Maggi Corner</h2>

            <p>
                Enjoy delicious, hot and freshly prepared Maggi
                with your friends and family.
            </p>

            <button>Order Now</button>

        </div>

    </section>


    <!-- About Section -->
    <section id="about" class="about">

        <h2>About Us</h2>

        <p>
            Maggi Corner is a cozy place for Maggi lovers.
            We serve freshly prepared and tasty Maggi with
            different flavours and delicious toppings.
        </p>

    </section>


    <!-- Menu Section -->
    <section id="menu">

        <h2>Our Maggi Menu</h2>

        <div class="menu-container">


            <!-- Card 1 -->
            <div class="food-card">

                <img
                    src="https://images.unsplash.com/photo-1585032226651-759b368d7246"
                    alt="Classic Maggi">

                <h3>Classic Masala Maggi</h3>

                <p>
                    Hot and spicy classic masala Maggi.
                </p>

                <h4>₹60</h4>

              <button onclick="openOrder('Classic Masala Maggi', 60)">Order Now</button>  

            </div>


            <!-- Card 2 -->
            <div class="food-card">

                <img
                    src="https://images.unsplash.com/photo-1552611052-33e04de081de"
                    alt="Cheese Maggi">

                <h3>Cheese Maggi</h3>

                <p>
                    Creamy and cheesy Maggi with extra cheese.
                </p>

                <h4>₹90</h4>

                <button onclick="openOrder('Cheese Maggi', 90)">Order Now</button>

            </div>


            <!-- Card 3 -->
            <div class="food-card">

                <img
                    src="https://images.unsplash.com/photo-1569718212165-3a8278d5f624"
                    alt="Spicy Maggi">

                <h3>Spicy Schezwan Maggi</h3>

                <p>
                    Spicy Maggi loaded with Schezwan flavour.
                </p>

                <h4>₹80</h4>

                <button onclick="openOrder('Spicy Schezwan Maggi', 80)">Order Now</button>

            </div>


            <!-- Card 4 -->
            <div class="food-card">

                <img
                    src="https://images.unsplash.com/photo-1585032226651-759b368d7246"
                    alt="Veg Maggi">

                <h3>Veggie Maggi</h3>

                <p>
                    Delicious Maggi with fresh vegetables.
                </p>

                <h4>₹75</h4>

                <button onclick="openOrder('Veggie Maggi', 75)">Order Now</button>

            </div>

        </div>

    </section>


    <!-- Offers Section -->
    <section id="offers" class="offers">

        <h2>Special Offer</h2>

        <div class="offer-box">

            <h3>Maggi Combo</h3>

            <p>
                Get 2 Classic Maggi + 2 Cold Drinks at just ₹150!
            </p>

            <button>Grab Offer</button>

        </div>

    </section>


    <!-- Contact Section -->
    <section id="contact" class="contact">

        <h2>Contact Us</h2>

        <p><strong>Address:</strong> Main Market, Kanpur</p>

        <p><strong>Phone:</strong> +91 9876543210</p>

        <p><strong>Email:</strong> maggicorner@example.com</p>

    </section>


    <!-- Footer -->
    <footer>

        <p>© 2026 Maggi Corner. All Rights Reserved.</p>

    </footer>
<!-- Order Form -->

<div id="orderModal" class="modal">

    <div class="order-box">

        <span class="close" onclick="closeOrder()">&times;</span>

        <h2>🍜 Place Your Order</h2>

        <form onsubmit="placeOrder(event)">

            <label>Selected Item</label>
            <input type="text" id="selectedItem" readonly>

            <label>Price</label>
            <input type="text" id="itemPrice" readonly>

            <label>Quantity</label>
            <input type="number" id="quantity"
                   value="1" min="1"
                   onchange="calculateTotal()">

            <label>Your Name</label>
            <input type="text" id="customerName"
                   placeholder="Enter your name" required>

            <label>Phone Number</label>
            <input type="tel" id="phone"
                   placeholder="Enter phone number" required>

            <label>Address</label>
            <textarea id="address"
                      placeholder="Enter your address"
                      required></textarea>

            <h3>Total: ₹<span id="totalPrice">0</span></h3>

            <button type="submit">Place Order</button>

        </form>

    </div>

</div>


<!-- Confirmation -->

<div id="successMessage" class="success">

    <div class="success-box">

        <h2>✅ Order Confirmed!</h2>

        <p id="confirmationText"></p>

        <button onclick="closeSuccess()">Done</button>

    </div>

</div>

<script>
let currentPrice = 0;

function openOrder(item, price) {

    currentPrice = price;

    document.getElementById("selectedItem").value = item;
    document.getElementById("itemPrice").value = "₹" + price;

    document.getElementById("quantity").value = 1;

    calculateTotal();

    document.getElementById("orderModal").style.display = "flex";
}


function calculateTotal() {

    let quantity =
        document.getElementById("quantity").value;

    let total = currentPrice * quantity;

    document.getElementById("totalPrice").innerText = total;
}


function closeOrder() {

    document.getElementById("orderModal").style.display = "none";
}


function placeOrder(event) {

    event.preventDefault();

    let name =
        document.getElementById("customerName").value;

    let item =
        document.getElementById("selectedItem").value;

    let quantity =
        document.getElementById("quantity").value;

    let total =
        document.getElementById("totalPrice").innerText;

    document.getElementById("orderModal").style.display = "none";

    document.getElementById("confirmationText").innerText =
        "Thank you " + name +
        "! Your order of " +
        quantity + " × " +
        item +
        " has been placed. Total: ₹" +
        total;

    document.getElementById("successMessage").style.display = "flex";
}


function closeSuccess() {

    document.getElementById("successMessage").style.display = "none";
}
</script>
</body>
</html>
