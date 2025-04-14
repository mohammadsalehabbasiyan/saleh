<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tech Heim - Digital Store</title>
    <style>
        /* Reset Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }
        
        /* Header Styles */
  header {
            background-color: white;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            padding: 20px 0;
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
  .header-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 20px;
        }
        
  .logo {
            font-size: 2rem;
            font-weight: bold;
            color: black;
            text-decoration: none;
        }
        
  nav ul {
            display: flex;
            list-style: none;
        }
        
  nav ul li {
            margin-left: 30px;
        }
        
  nav ul li a {
            text-decoration: none;
            color: #333;
            font-weight: 500;
            transition: color 0.3s;
        }
        
  nav ul li a:hover {
            color: #ff6b00;
        }
        
   .account-cart {
            display: flex;
            align-items: center;
        }
        
   .account-cart a {
            margin-left: 20px;
            text-decoration: none;
            color: #333;
        }
        
        /* Hero Section */
   .hero {
            text-align: center;
            padding: 80px 20px;
        }
        
  .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
            color: black;
        }
        
  .search-bar {
            margin: 30px auto;
            max-width: 600px;
        }
        
  .search-bar input {
            width: 100%;
            padding: 15px 20px;
            border: 1px solid #ddd;
            border-radius: 30px;
            font-size: 1rem;
            outline: none;
        }
        
        /* Products Section */
  .products-section {
            max-width: 1200px;
            margin: 50px auto;
            padding: 0 20px;
        }
        
   .section-title {
            text-align: center;
            margin-bottom: 40px;
            font-size: 2rem;
        }
        
  .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 30px;
        }
        
  .product-card {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s;
        }
        
   .product-card:hover {
            transform: translateY(-10px);
        }
        
   .product-image {
            height: 200px;
            background-color: #f5f5f5;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
   .product-info {
            padding: 20px;
        }
        
  .product-title {
            font-size: 1.2rem;
            margin-bottom: 10px;
        }
        
   .product-price {
            font-weight: bold;
            color: #ff6b00;
            font-size: 1.3rem;
            margin-bottom: 15px;
        }
        
  .add-to-cart {
            display: block;
            width: 100%;
            padding: 12px;
            background-color: #ff6b00;
            color: white;
            border: none;
            border-radius: 5px;
            font-weight: bold;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        
   .add-to-cart:hover {
            background-color: #e05d00;
        }
        
        /* Skip Button */
  .skip-button {
            position: fixed;
            bottom: 30px;
            right: 30px;
            padding: 12px 25px;
            background-color: #ff6b00;
            color: white;
            border: none;
            border-radius: 30px;
            font-weight: bold;
            cursor: pointer;
            box-shadow: 0 5px 15px rgba(255, 107, 0, 0.3);
            z-index: 10;
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="header-container">
            <a href="#" class="logo">Tech Heim</a>
            
  <nav>
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Products</a></li>
                    <li><a href="#">Categories</a></li>
                    <li><a href="#">Deals</a></li>
                    <li><a href="#">About</a></li>
                    <li><a href="#">Contact</a></li>
                </ul>
            </nav>
            
  <div class="account-cart">
                <a href="#">Account</a>
                <a href="#">Cart (0)</a>
            </div>
        </div>
    </header>
    <!-- Hero Section -->
    <section class="hero">
        <h1>Tech Heim</h1>
        <div class="search-bar">
            <input type="text" placeholder="Search products...">
        </div>
    </section>
    <!-- Products Section -->
    <section class="products-section">
        <h2 class="section-title">Featured Products</h2>
        
  <div class="products-grid">
            <!-- Product 1 -->
            <div class="product-card">
                <div class="product-image">
                    <img src="https://via.placeholder.com/250" alt="Product 1">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Wireless Headphones</h3>
                    <p class="product-price">$99.99</p>
                    <button class="add-to-cart">Add to Cart</button>
                </div>
            </div>
            <!-- Product 2 -->
            <div class="product-card">
                <div class="product-image">
                    <img src="https://via.placeholder.com/250" alt="Product 2">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Smart Watch</h3>
                    <p class="product-price">$199.99</p>
                    <button class="add-to-cart">Add to Cart</button>
                </div>
            </div>
            <!-- Product 3 -->
            <div class="product-card">
                <div class="product-image">
                    <img src="https://via.placeholder.com/250" alt="Product 3">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Bluetooth Speaker</h3>
                    <p class="product-price">$79.99</p>
                    <button class="add-to-cart">Add to Cart</button>
                </div>
            </div>
            <!-- Product 4 -->
            <div class="product-card">
                <div class="product-image">
                    <img src="https://via.placeholder.com/250" alt="Product 4">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Laptop Stand</h3>
                    <p class="product-price">$49.99</p>
                    <button class="add-to-cart">Add to Cart</button>
                </div>
            </div>
        </div>
    </section>
    <!-- Skip Button -->
    <button class="skip-button">Skip</button>
</body>
</html>
