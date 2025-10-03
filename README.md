# **Fashion Store Project**

# Overview
The Fashion Store project is divided into two parts:

1. **Justine-Frontend** – A user-friendly fashion store website that showcases different fashion options, upcoming sales, and benefits of purchasing.  
2. **Dior-Backend** – Extends the fashion store with a database to track inventory, sales, and revenue.  

---

# Justine-Frontend

# Description
- Displays fashion products in a grid layout.  
- Shows upcoming sale offers in a structured table.  
- Includes a footer with copyright marks.  

# Technologies Used
- HTML5  
- CSS3  

# Files
- `Justine-Frontend/index.html`  
- `Justine-Frontend/style.css`  

# How to Run
1. Download the repo.  
2. Open `Justine-Frontend/index.html` in your browser.  

# Due Date
**1 October 2025**  

---

# Dior-Backend

# Description
- Tracks store inventory and sales data.  
- Displays:
  - Total stock  
  - Items sold  
  - Remaining stock  
  - Revenue earned  

# Technologies Used
- Node.js  
- Express.js  
- SQLite  

# Files
- `Dior-Backend/server.js`  
- `Dior-Backend/fashion.sql`  

# How to Run
1. Install dependencies:
   ```bash
   npm install express sqlite
   sqlite3 fashion.db < Dior-Backend/fashion.sql
   node Dior-Backend/server.js
   http://localhost:3000/inventory
   
