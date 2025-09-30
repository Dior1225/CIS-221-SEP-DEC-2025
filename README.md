# CIS-221-SEP-DEC-2025
For learning

# HTML + CSS + Inventory Template
template = """
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Fashion Store</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      background-color: #fdf6f0;
      color: #333;
    }
    header {
      background-color: #ff6f61;
      color: white;
      padding: 20px;
      text-align: center;
    }
    .product-grid {
      display: flex;
      gap: 20px;
      padding: 20px;
      flex-wrap: wrap;
      justify-content: center;
    }
    .product {
      background-color: white;
      border: 1px solid #ddd;
      padding: 10px;
      width: 200px;
      text-align: center;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    .sales table, .inventory table {
      width: 90%;
      margin: 20px auto;
      border-collapse: collapse;
    }
    th, td {
      border: 1px solid #ccc;
      padding: 10px;
      text-align: center;
    }
    th {
      background-color: #ffe0dc;
    }
    .benefits {
      text-align: center;
      font-style: italic;
      margin: 10px;
    }
    footer {
      background-color: #ff6f61;
      color: white;
      text-align: center;
      padding: 10px;
    }
  </style>
</head>
<body>
  <header>
    <h1>Fashion Store</h1>
    <p>Your one-stop shop for trendy fashion</p>
  </header>

  <section class="products">
    <h2>Featured Fashion</h2>
    <div class="product-grid">
      <div class="product">
        <img src="https://via.placeholder.com/200x250?text=Elegant+Dress" alt="Elegant Dress" />
        <h3>Elegant Dress</h3>
        <p>$49.99</p>
      </div>
      <div class="product">
        <img src="https://via.placeholder.com/200x250?text=Stylish+Jacket" alt="Stylish Jacket" />
        <h3>Stylish Jacket</h3>
        <p>$89.99</p>
      </div>
    </div>
  </section>

  <section class="sales">
    <h2>Upcoming Sale Offers</h2>
    <table>
      <tr>
        <th>Sale Name</th>
        <th>Start Date</th>
        <th>Discount</th>
        <th>Details</th>
      </tr>
      <tr>
        <td>Autumn Bonanza</td>
        <td>Oct 5, 2025</td>
        <td>30% Off</td>
        <td>On all jackets and coats</td>
      </tr>
      <tr>
        <td>Festive Flash Sale</td>
        <td>Oct 15, 2025</td>
        <td>50% Off</td>
        <td>Selected dresses and accessories</td>
      </tr>
    </table>
    <p class="benefits">
      Shopping with Fashion Store means exclusive styles, fast delivery, and unbeatable prices. Join our fashion family today!
    </p>
  </section>

  <section class="inventory">
    <h2>  Inventory Tracker</h2>
    <table>
      <tr>
        <th>Item</th><th>Price</th><th>Bought</th><th>Sold</th><th>In Stock</th><th>Revenue</th>
      </tr>
      {% for item in items %}
      <tr>
        <td>{{ item.name }}</td>
        <td>${{ item.price }}</td>
        <td>{{ item.bought }}</td>
        <td>{{ item.sold }}</td>
        <td>{{ item.stock }}</td>
        <td>${{ item.revenue }}</td>
      </tr>
      {% endfor %}
    </table>
    <h3 style="text-align:center;">Total Revenue: ${{ total }}</h3>
  </section>

  <footer>
    <p>&copy; 2025 Fashion Store. All rights reserved.</p>
  </footer>
</body>
</html>
"""

#  Fashion Store – CIS-221 Project

This is a learning project for CIS-221 (SEP–DEC 2025). It showcases fashion items, upcoming sales, and tracks inventory using a database.

---

##  Features

-  Product grid with images and prices
-  Upcoming sale offers in a structured table
-  Inventory tracking (items bought, sold, in stock, revenue)
-  Eye-catching design with CSS
-  Backend powered by Flask and SQLite

---

##  File Overview

| File            | Purpose                                      |
|-----------------|----------------------------------------------|
| `app.py`        | Flask app with embedded HTML/CSS template    |
| `fashion.db`    | SQLite database storing inventory data       |
| `README.md`     | Project description and setup instructions   |

---

1. Clone the repository:
   ```bash
   git clone https://github.com/Dior1225/CIS-221-SEP-DEC-2025.git
   cd CIS-221-SEP-DEC-2025

2. Install Flask:
   ```bash
   pip install flask

python app.py

http://127.0.0.1:5000/
