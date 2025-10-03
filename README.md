# **Fashion Store Project**

# Overview
The Fashion Store project is divided into two parts:

1. **Part 1 (Frontend)** – A user-friendly fashion store website that showcases different fashion options, upcoming sales, and benefits of purchasing.  
2. **Part 2 (Backend + Database)** – Extends the fashion store with a database to track inventory, sales, and revenue.  

---

# Part 1: Frontend

# Description
- Displays fashion products in a grid layout.  
- Shows upcoming sale offers in a structured table.  
- Includes a footer with copyright marks.  

# Technologies Used
- HTML5  
- CSS3  

# Files
- `part1/index.html`  
- `part1/style.css`  

# How to Run
1. Download the repo.  
2. Open `part1/index.html` in your browser.

# Part 2: Backend + Database

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
- `part2/server.js`  
- `part2/fashion.sql`  

# How to Run
1. Install dependencies:
   ```bash
   npm install express sqlite3

   sqlite3 fashion.db < part2/fashion.sql

   node part2/server.js

   http://localhost:3000/inventory
