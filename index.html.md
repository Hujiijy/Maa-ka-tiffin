#   
<!DOCTYPE html>  
<html lang="en">  
<head>  
<meta charset="UTF-8">  
<meta name="viewport" content="width=device-width, initial-scale=1.0">  
<title>Maa Ka Tiffin</title>  
  
<!-- Google Font -->  
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">  
  
<style>  
* {  
    margin: 0;  
    padding: 0;  
    box-sizing: border-box;  
    font-family: 'Poppins', sans-serif;  
}  
  
body {  
    background: #f9fafc;  
    color: #333;  
}  
  
/* Navbar */  
nav {  
    display: flex;  
    justify-content: space-between;  
    padding: 15px 50px;  
    background: white;  
    box-shadow: 0 2px 10px rgba(0,0,0,0.05);  
    position: sticky;  
    top: 0;  
}  
  
nav h2 {  
    color: #ff5a3c;  
}  
  
nav a {  
    text-decoration: none;  
    margin: 0 10px;  
    color: #333;  
    font-weight: 500;  
}  
  
/* Hero Section */  
.hero {  
    display: flex;  
    justify-content: space-between;  
    align-items: center;  
    padding: 60px 50px;  
}  
  
.hero-text {  
    max-width: 500px;  
}  
  
.hero h1 {  
    font-size: 40px;  
    margin-bottom: 15px;  
}  
  
.hero p {  
    margin-bottom: 20px;  
    color: #666;  
}  
  
.btn {  
    padding: 12px 20px;  
    background: #25D366;  
    color: white;  
    border: none;  
    border-radius: 8px;  
    cursor: pointer;  
    font-size: 16px;  
}  
  
.hero img {  
    width: 350px;  
}  
  
/* Section */  
section {  
    padding: 50px;  
}  
  
/* Menu */  
.menu {  
    display: grid;  
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));  
    gap: 20px;  
}  
  
.card {  
    background: white;  
    padding: 20px;  
    border-radius: 15px;  
    box-shadow: 0 5px 15px rgba(0,0,0,0.05);  
}  
  
.card h3 {  
    margin-bottom: 10px;  
}  
  
.price {  
    color: #ff5a3c;  
    font-weight: bold;  
}  
  
/* Features */  
.features {  
    display: flex;  
    justify-content: space-around;  
    text-align: center;  
}  
  
.feature-box {  
    max-width: 200px;  
}  
  
/* Footer */  
footer {  
    background: #333;  
    color: white;  
    text-align: center;  
    padding: 20px;  
}  
  
/* Mobile */  
@media(max-width: 768px) {  
    .hero {  
        flex-direction: column;  
        text-align: center;  
    }  
  
    nav {  
        padding: 15px;  
    }  
}  
</style>  
</head>  
  
<body>  
  
<!-- Navbar -->  
<nav>  
    <h2>🍱 Maa Ka Tiffin</h2>  
    <div>  
        <a href="#">Home</a>  
        <a href="#menu">Menu</a>  
        <a href="#contact">Contact</a>  
    </div>  
</nav>  
  
<!-- Hero -->  
<div class="hero">  
    <div class="hero-text">  
        <h1>Fresh Homemade Food Delivered Daily</h1>  
        <p>Healthy, hygienic and affordable meals made with love. Perfect for students & working professionals.</p>  
        <button class="btn" onclick="orderNow()">Order on WhatsApp</button>  
    </div>  
    <img src="https://cdn-icons-png.flaticon.com/512/1046/1046784.png">  
</div>  
  
<!-- Features -->  
<section>  
    <h2>Why Choose Us</h2>  
    <div class="features">  
        <div class="feature-box">  
            <h4>🥗 Healthy</h4>  
            <p>Balanced homemade meals</p>  
        </div>  
        <div class="feature-box">  
            <h4>🚚 Fast Delivery</h4>  
            <p>On-time daily delivery</p>  
        </div>  
        <div class="feature-box">  
            <h4>💰 Affordable</h4>  
            <p>Budget-friendly pricing</p>  
        </div>  
    </div>  
</section>  
  
<!-- Menu -->  
<section id="menu">  
    <h2>Our Menu</h2>  
    <div class="menu">  
        <div class="card">  
            <h3>Basic Veg Tiffin</h3>  
            <p>4 Roti + Sabzi + Dal + Rice</p>  
            <p class="price">₹80 / meal</p>  
        </div>  
  
        <div class="card">  
            <h3>Special Tiffin</h3>  
            <p>Paneer + Roti + Rice + Sweet</p>  
            <p class="price">₹120 / meal</p>  
        </div>  
  
        <div class="card">  
            <h3>Monthly Plan</h3>  
            <p>Lunch + Dinner (30 days)</p>  
            <p class="price">₹4500</p>  
        </div>  
    </div>  
</section>  
  
<!-- Contact -->  
<section id="contact">  
    <h2>Order Now</h2>  
    <p>Click below to place your order instantly</p>  
    <button class="btn" onclick="orderNow()">Order on WhatsApp</button>  
</section>  
  
<!-- Footer -->  
<footer>  
    <p>📞 9876543210 | 📍 Your City</p>  
</footer>  
  
<script>  
function orderNow() {  
    let phone = "919876543210"; // change this  
    let message = "Hello, I want to order tiffin.";  
    let url = "https://wa.me/" + phone + "?text=" + encodeURIComponent(message);  
    window.open(url, "_blank");  
}  
</script>  
  
</body>  
</html>  
