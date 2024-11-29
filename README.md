# Success-storesdocument.getElementById('contactForm').addEventListener('submit', function (e) {
    e.preventDefault();
    alert('Thank you for contacting SuccessX Stores! We will get back to you soon.');
});/* General Reset */
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
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 2rem;
    background-color: #222;
    color: #fff;
}

header .logo {
    font-size: 1.5rem;
    font-weight: bold;
}

header nav ul {
    list-style: none;
    display: flex;
    gap: 1.5rem;
}

header nav ul li a {
    color: #fff;
    text-decoration: none;
}

/* Hero Section */
.hero {
    background: url('https://via.placeholder.com/1920x600') no-repeat center center/cover;
    color: #fff;
    text-align: center;
    padding: 5rem 1rem;
}

.hero-content h1 {
    font-size: 3rem;
    margin-bottom: 1rem;
}

.hero-content .btn {
    padding: 0.5rem 1.5rem;
    background-color: #007bff;
    color: #fff;
    text-decoration: none;
    border-radius: 5px;
}

/* Gallery */
.gallery {
    padding: 2rem 1rem;
    background-color: #f8f9fa;
}

.gallery h2 {
    text-align: center;
    margin-bottom: 1rem;
}

.gallery .grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 1rem;
}

.gallery .item {
    text-align: center;
    background: #fff;
    padding: 1rem;
    border-radius: 5px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

.gallery .item img {
    width: 100%;
    border-radius: 5px;
}

/* Contact */
.contact {
    padding: 2rem 1rem;
    background-color: #222;
    color: #fff;
    text-align: center;
}

.contact h2 {
    margin-bottom: 1rem;
}

.contact form {
    max-width: 500px;
    margin: 0 auto;
    text-align: left;
}

.contact form label {
    display: block;
    margin-bottom: 0.5rem;
}

.contact form input,
.contact form textarea,
.contact form button {
    width: 100%;
    margin-bottom: 1rem;
    padding: 0.5rem;
    border: none;
    border-radius: 5px;
}

.contact form button {
    background-color: #007bff;
    color: #fff;
    cursor: pointer;
}

.contact form button:hover {
    background-color: #0056b3;
}

/* Footer */
footer {
    text-align: center;
    padding: 1rem;
    background-color: #111;
    color: #fff;
}

/* Responsive */
@media (max-width: 768px) {
    header {
        flex-direction: column;
        text-align: center;
    }

    header nav ul {
        flex-direction: column;
    }
}<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SuccessX Stores</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <div class="logo">SuccessX Stores</div>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#gallery">Gallery</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="home" class="hero">
        <div class="hero-content">
            <h1>Welcome to SuccessX Stores</h1>
            <p>Your ultimate destination for premium products!</p>
            <a href="#gallery" class="btn">Browse Products</a>
        </div>
    </section>

    <section id="gallery" class="gallery">
        <h2>Our Products</h2>
        <div class="grid">
            <div class="item"><img src="https://via.placeholder.com/300" alt="Product 1"><p>Luxury Watch</p></div>
            <div class="item"><img src="https://via.placeholder.com/300" alt="Product 2"><p>Designer Handbag</p></div>
            <div class="item"><img src="https://via.placeholder.com/300" alt="Product 3"><p>Smartphone</p></div>
            <div class="item"><img src="https://via.placeholder.com/300" alt="Product 4"><p>Sports Shoes</p></div>
        </div>
    </section>

    <section id="contact" class="contact">
        <h2>Contact SuccessX Stores</h2>
        <form id="contactForm">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
            
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            
            <label for="message">Message:</label>
            <textarea id="message" name="message" rows="5" required></textarea>
            
            <button type="submit">Send</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2024 SuccessX Stores. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
