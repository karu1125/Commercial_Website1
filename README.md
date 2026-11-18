# Ex02 Commercial Website
## Date: 18/11/2026

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
### index.html
```.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ShopEase - Online Shopping</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <nav class="navbar">
            <h1 class="logo">ShopEase</h1>

            <div class="nav-links">
                <a href="#">Home</a>
                <a href="#">Products</a>
                <a href="#">Categories</a>
                <a href="#">Offers</a>
                <a href="#">Contact</a>
            </div>
        </nav>
    </header>

    <section class="hero">
        <div class="hero-content">
            <h2>Discover Your Style</h2>
            <p>Shop the latest trends at amazing prices.</p>
            <a href="#products" class="shop-btn">Shop Now</a>
        </div>
    </section>

    <section class="categories">
        <h2>Shop By Category</h2>

        <div class="category-container">
            <div class="category">Fashion</div>
            <div class="category">Electronics</div>
            <div class="category">Accessories</div>
            <div class="category">Footwear</div>
        </div>
    </section>

    <section class="products" id="products">
        <h2>Featured Products</h2>

        <div class="product-container">

            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1523275335684-37898b6baf30?w=500" alt="Watch">
                <h3>Classic Watch</h3>
                <p>₹1,499</p>
                <button>Buy Now</button>
            </div>

            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1505740420928-5e560c06d30e?w=500" alt="Headphones">
                <h3>Wireless Headphones</h3>
                <p>₹2,499</p>
                <button>Buy Now</button>
            </div>

            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1542291026-7eec264c27ff?w=500" alt="Shoes">
                <h3>Sports Shoes</h3>
                <p>₹1,999</p>
                <button>Buy Now</button>
            </div>

            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1548036328-c9fa89d128fa?w=500" alt="Bag">
                <h3>Stylish Handbag</h3>
                <p>₹1,799</p>
                <button>Buy Now</button>
            </div>

        </div>
    </section>

    <section class="offer">
        <h2>Special Festival Sale!</h2>
        <p>Get up to 50% OFF on selected products.</p>
        <a href="#products">Explore Offers</a>
    </section>

    <footer>
        <h2>ShopEase</h2>
        <p>Your Style, Your Choice, Your Shopping Destination.</p>
        <p>© 2026 ShopEase. All Rights Reserved.</p>
    </footer>

</body>
</html>
```

### style.css
```.css

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

body {
    background-color: #f5f5f5;
    color: #333;
}

.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 8%;
    background-color: #222;
    color: white;
}

.logo {
    color: #ffb703;
    font-size: 28px;
}

.nav-links {
    display: flex;
    gap: 30px;
}

.nav-links a {
    color: white;
    text-decoration: none;
    font-size: 16px;
}

.nav-links a:hover {
    color: #ffb703;
}

.hero {
    height: 350px;
    background: linear-gradient(90deg, #222, #555);
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    color: white;
}

.hero-content h2 {
    font-size: 42px;
    margin-bottom: 15px;
}

.hero-content p {
    font-size: 18px;
    margin-bottom: 25px;
}

.shop-btn {
    display: inline-block;
    background-color: #ffb703;
    color: #222;
    padding: 12px 25px;
    text-decoration: none;
    border-radius: 5px;
    font-weight: bold;
}

.categories {
    padding: 40px 8%;
    text-align: center;
}

.categories h2,
.products h2 {
    margin-bottom: 25px;
    font-size: 28px;
}

.category-container {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
}

.category {
    background-color: white;
    padding: 25px 45px;
    border-radius: 8px;
    font-weight: bold;
    box-shadow: 0 3px 10px #ddd;
}

.products {
    padding: 40px 8%;
    text-align: center;
}

.product-container {
    display: flex;
    justify-content: center;
    gap: 25px;
    flex-wrap: wrap;
}

.product-card {
    background-color: white;
    width: 230px;
    padding: 15px;
    border-radius: 10px;
    box-shadow: 0 3px 12px #ddd;
    transition: transform 0.3s;
}

.product-card:hover {
    transform: translateY(-8px);
}

.product-card img {
    width: 100%;
    height: 180px;
    object-fit: cover;
    border-radius: 8px;
}

.product-card h3 {
    margin: 15px 0 10px;
}

.product-card p {
    color: #e63946;
    font-size: 19px;
    font-weight: bold;
    margin-bottom: 15px;
}

.product-card button {
    background-color: #222;
    color: white;
    border: none;
    padding: 10px 25px;
    border-radius: 5px;
    cursor: pointer;
}

.product-card button:hover {
    background-color: #ffb703;
    color: #222;
}

.offer {
    background-color: #ffb703;
    text-align: center;
    padding: 45px 20px;
}

.offer h2 {
    font-size: 30px;
    margin-bottom: 12px;
}

.offer p {
    margin-bottom: 20px;
}

.offer a {
    display: inline-block;
    background-color: #222;
    color: white;
    padding: 12px 25px;
    text-decoration: none;
    border-radius: 5px;
}

footer {
    background-color: #222;
    color: white;
    text-align: center;
    padding: 30px;
}

footer h2 {
    color: #ffb703;
    margin-bottom: 10px;
}

footer p {
    margin: 8px;
}

@media (max-width: 650px) {
    .navbar {
        flex-direction: column;
        gap: 15px;
    }

    .nav-links {
        flex-wrap: wrap;
        justify-content: center;
        gap: 15px;
    }

    .hero-content h2 {
        font-size: 30px;
    }
}

```

## OUTPUT
<img width="1917" height="1092" alt="image" src="https://github.com/user-attachments/assets/c6110e76-4126-4e5e-a868-84abc0e6a9be" />

<img width="1917" height="1093" alt="image" src="https://github.com/user-attachments/assets/ed0db05b-6a92-46b2-930f-51f2dc7883d5" />


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
