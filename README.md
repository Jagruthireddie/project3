# project3
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Product Page</title>
  <style>
    /* General Reset */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, sans-serif;
      background-color: #f4f4f4;
      line-height: 1.6;
    }

    /* Navigation Bar */
    nav {
      background-color: #333;
      color: #fff;
      padding: 15px 20px;
      text-align: center;
    }

    nav a {
      color: #fff;
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
    }

    nav a:hover {
      text-decoration: underline;
    }

    /* Main Content Area */
    .container {
      display: flex;
      justify-content: space-between;
      padding: 50px;
      max-width: 1200px;
      margin: 0 auto;
    }

    .product-image {
      flex: 1;
      max-width: 700px;
      margin-right: 50px;
      border-radius: 8px;
      box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
      overflow: hidden;
    }

    .product-image img {
      width: 100%;
      height: auto;
      transition: transform 0.3s ease-in-out;
    }

    .product-image img:hover {
      transform: scale(1.1);
    }

    .product-details {
      flex: 1;
      max-width: 500px;
    }

    .product-details h1 {
      font-size: 2.5rem;
      color: #333;
      margin-bottom: 20px;
    }

    .product-details p {
      font-size: 1rem;
      color: #666;
      margin-bottom: 20px;
    }

    .product-details .price {
      font-size: 1.8rem;
      font-weight: bold;
      color: #e60000;
      margin-bottom: 20px;
    }

    .product-details .add-to-cart {
      background-color: #e60000;
      color: #fff;
      padding: 15px;
      font-size: 1.2rem;
      border: none;
      cursor: pointer;
      width: 100%;
      transition: background-color 0.3s;
      border-radius: 5px;
    }

    .product-details .add-to-cart:hover {
      background-color: #cc0000;
    }

    /* Product Image Gallery */
    .gallery {
      display: flex;
      justify-content: center;
      margin-top: 30px;
    }

    .gallery img {
      width: 70px;
      height: 70px;
      margin: 0 10px;
      cursor: pointer;
      border-radius: 5px;
      transition: transform 0.3s;
    }

    .gallery img:hover {
      transform: scale(1.1);
    }

    /* Customer Reviews Section */
    .reviews {
      padding: 50px;
      background-color: #fff;
      margin-top: 30px;
    }

    .reviews h2 {
      font-size: 2rem;
      color: #333;
      margin-bottom: 15px;
    }

    .reviews p {
      font-size: 1rem;
      color: #666;
    }

    .reviews .rating {
      font-size: 1.5rem;
      color: #f7b500;
    }

    /* Related Products Section */
    .related-products {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      margin-top: 50px;
      padding: 50px 0;
      background-color: #f4f4f4;
    }

    .related-products h2 {
      font-size: 2rem;
      color: #333;
      text-align: center;
      width: 100%;
      margin-bottom: 30px;
    }

    .related-product {
      flex: 1;
      max-width: 400px;
      margin: 50px;
      background-color: #fff;
      box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
      border-radius: 8px;
      overflow: hidden;
      text-align: center;
      padding: 30px;
    }

    .related-product img {
      width: 100%;
      height: 400px;
      object-fit: cover;
      transition: transform 0.3s;
    }

    .related-product img:hover {
      transform: scale(1.05);
    }

    .related-product .price {
      font-size: 1.4rem;
      color: #e60000;
      font-weight: bold;
      margin-top: 15px;
    }

    /* Responsive Design */
    @media (max-width: 768px) {
      .container {
        flex-direction: column;
        align-items: center;
      }

      .product-image {
        margin-right: 0;
        margin-bottom: 20px;
      }

      .product-details {
        max-width: 100%;
      }

      .related-products {
        flex-direction: column;
        align-items: center;
      }

      .related-product {
        margin-bottom: 30px;
      }
    }

  </style>
</head>
<body>

  <!-- Navigation Bar -->
  <nav>
    <a href="#">Home</a>
    <a href="#">Shop</a>
    <a href="#">Contact</a>
  </nav>

  <!-- Product Page -->
  <div class="container">
    <!-- Product Image -->
    <div class="product-image">
      <img src="https://redtape.com/cdn/shop/products/8-800x800_22c88bd9-f9c2-4c61-ab55-71edce92bf57.jpg?v=1738414416" alt="Product Image">
      
    </div>

    <!-- Product Details -->
    <div class="product-details">
      <h1>Stylish Running Shoes</h1>
      <p>This stylish pair of running shoes is perfect for daily workouts, jogging, or casual wear. Made with breathable materials and a durable rubber sole, these shoes are designed to provide maximum comfort and support throughout the day. Whether you're running, walking, or just lounging, this footwear is sure to meet your needs.</p>
      <p class="price">$99.99</p>
      <button class="add-to-cart">Add to Cart</button>
    </div>
  </div>

  <!-- Customer Reviews Section -->
  <section class="reviews">
    <h2>Customer Reviews</h2>
    <p class="rating">★★★★☆</p>
    <p>This product is amazing! Highly recommend it! The fit is perfect and they are super comfortable!</p>
  </section>

  <!-- Related Products Section -->
  <section class="related-products">
    <h2>Related Products</h2>
    <div class="related-product">
      <img src="https://rukminim2.flixcart.com/image/850/1000/xif0q/shoe/0/c/3/6-rng-854-grey-40-bruton-grey-original-imah3xh6a6ecvmng.jpeg?q=90&crop=false" alt="Related Product">
      <p class="price">$79.99</p>
    </div>
    <div class="related-product">
      <img src="https://rukminim2.flixcart.com/image/850/1250/xif0q/shoe/t/6/w/9-vs-9500-9-world-wear-footwear-white-original-imagn6a5fqbncryj.jpeg?q=90&crop=false" alt="Related Product">
      <p class="price">$59.99</p>
    </div>
    <div class="related-product">
      <img src="https://redtape.com/cdn/shop/files/RSO3495_1.jpg?v=1738408782" alt="Related Product">
      <p class="price">$89.99</p>
    </div>
  </section>

</body>
</html>
