<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Online Store</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        header {
            background-color: #333;
            color: #fff;
            padding: 10px;
            text-align: center;
        }

        .product {
            border: 1px solid #ddd;
            border-radius: 5px;
            padding: 10px;
            margin: 10px;
            background-color: #fff;
            box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
        }

        button {
            background-color: #4CAF50;
            color: #fff;
            padding: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        button:hover {
            background-color: #45a049;
        }

        #cart {
            text-align: right;
            padding: 10px;
            background-color: #ddd;
            cursor: pointer;
            position: fixed;
            top: 0;
            right: 0;
        }

        #cart-count {
            font-weight: bold;
            color: #333;
        }

        #product-page {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: #fff;
            padding: 20px;
            box-sizing: border-box;
        }

        #back-button {
            background-color: #333;
            color: #fff;
            padding: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        #product-details {
            margin-top: 20px;
        }

        #product-details img {
            max-width: 70px; /* Adjust this value for the desired size */
            height: auto;
        }
        
        .product img {
    max-width: 70px;
    height: auto;
}


        #cart-page {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: #fff;
            padding: 20px;
            box-sizing: border-box;
        }

        .cart-item {
            border-bottom: 1px solid #ddd;
            padding-bottom: 10px;
            margin-bottom: 10px;
            display: flex;
            align-items: center;
        }

        .cart-item img {
            max-width: 50px; /* Adjust this value for the desired size */
            height: auto;
            margin-right: 10px;
        }

        .remove-button {
            background-color: #ff0000;
            color: #fff;
            padding: 5px;
            border: none;
            border-radius: 3px;
            cursor: pointer;
            margin-left: auto;
        }
    </style>
</head>
<body>
    <header>
        <h1>Online Store</h1>
    </header>

    <div id="cart" onclick="showCartPage()">Cart: <span id="cart-count">0</span></div>

    <div id="products-container"></div>

    <div id="product-page">
        <button id="back-button" onclick="hideProductPage()">Back</button>
        <div id="product-details"></div>
    </div>

    <div id="cart-page">
        <button id="back-button" onclick="hideCartPage()">Back</button>
        <h2>Your Cart</h2>
        <div id="cart-items"></div>
        <p>Total: $<span id="cart-total">0</span></p>
    </div>

    <script>
        // Sample product data with images
        const products = [
            { id: 1, name: 'Apple Airpods', price: 99.99, image: 'Apple Airpods.png', description: 'Apple AirPods (2nd Generation) Wireless Ear Buds, Bluetooth Headphones with Lightning Charging Case Included, Over 24 Hours of Battery Life, Effortless Setup for iPhone' },
            { id: 2, name: '$19 Dollar fortnite card', price: 19, image: 'fortnite gift card14.jpeg', description: 'It is a $19 Dollar fornite card spend it on fortnite' },
            { id: 3, name: 'Grape-Kool-Aid', price: 36.69, image: 'perple cool aid.jpg', description: 'Kool-Aid Caffeine Free Grape Sweetened Powdered Drink Mix 12 Count 19 oz Canisters' },
        ];

        // Cart data
        const cart = [];

        // Render products
        const productsContainer = document.getElementById('products-container');
        products.forEach(product => {
            const productElement = document.createElement('div');
            productElement.className = 'product';
            productElement.innerHTML = `
                <h3>${product.name}</h3>
                <img src="${product.image}" alt="${product.name}">
                <p>Price: $${product.price}</p>
                <button onclick="addToCart(${product.id})">Add to Cart</button>
                <button onclick="showProductPage(${product.id})">Details</button>
            `;
            productsContainer.appendChild(productElement);
        });

        // Cart functionality
        const cartCountElement = document.getElementById('cart-count');
        const cartItemsContainer = document.getElementById('cart-items');
        const cartTotalElement = document.getElementById('cart-total');

        function addToCart(productId) {
            const product = products.find(p => p.id === productId);
            if (product) {
                cart.push(product);
                updateCartUI();
            }
        }

        function updateCartUI() {
            cartCountElement.textContent = cart.length;
            cartItemsContainer.innerHTML = '';
            let total = 0;

            cart.forEach((item, index) => {
                const cartItemElement = document.createElement('div');
                cartItemElement.className = 'cart-item';
                cartItemElement.innerHTML = `
                    <img src="${item.image}" alt="${item.name}">
                    <div>
                        <span>${item.name} - $${item.price}</span>
                        <button class="remove-button" onclick="removeFromCart(${index})">Remove</button>
                    </div>
                `;
                cartItemsContainer.appendChild(cartItemElement);

                total += item.price;
            });

            cartTotalElement.textContent = total;
        }

        function removeFromCart(index) {
            cart.splice(index, 1);
            updateCartUI();
        }

        // Cart page functionality
        const cartPage = document.getElementById('cart-page');

        function showCartPage() {
            cartPage.style.display = 'block';
            updateCartUI();
        }

        function hideCartPage() {
            cartPage.style.display = 'none';
        }

        // Product page functionality
        const productPage = document.getElementById('product-page');
        const productDetails = document.getElementById('product-details');

        function showProductPage(productId) {
            const product = products.find(p => p.id === productId);
            if (product) {
                productDetails.innerHTML = `
                    <h2>${product.name}</h2>
                    <img src="${product.image}" alt="${product.name}">
                    <p>Price: $${product.price}</p>
                    <p>${product.description}</p>
                `;
                productPage.style.display = 'block';
            }
        }

        function hideProductPage() {
            productPage.style.display = 'none';
        }
    </script>
</body>
</html>

