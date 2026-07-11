# FlavourMatch 🍽️

**FlavourMatch** is a premium, high-performance restaurant discovery and recommendation web application. It allows users to search, filter, compare, and discover the best culinary experiences across India from a database of over 29,500+ restaurants.

🔗 **Live Link:** [https://flavourmatch.vercel.app](https://flavourmatch.vercel.app)

---

## ✨ Features

### 🔍 1. Advanced Search & Filtering
- Search by restaurant name, city, or specific area/locality.
- Instantly filter by **Cuisine type**, **Budget limits** (Low, Mid, High), **Star Ratings**, and **Restaurant Type** (e.g., Casual Dining, Quick Bites, Dessert Parlor, etc.).
- Active filter chips allow users to easily review and remove filters dynamically.

### 🔢 2. High-Performance Pagination
- Custom-designed, light-themed pagination controls (`← Previous 1 2 3 ... Next →`) styled to match the primary branding.
- Selectable **Page Size** dropdown (12, 24, 50, or 100 results per page) with real-time recalculation of pages.
- Smooth scrolling mechanism that brings the user back to the top of the search grid after page changes.

### ⚖️ 3. Side-by-Side Comparison
- Add restaurants to a comparative list to compare their rating, average cost for two, location, cuisines, and types side-by-side on a dedicated comparison dashboard.

### 📋 4. Detailed Restaurant Profiles & Similar Finder
- Explore comprehensive information about individual restaurants.
- Dynamic **"Find Similar"** finder that highlights and recommends alternative dining options matching the cuisines and style of the selected restaurant.

### ⚡ 5. Dual Query System (Client-Side CSV & Server Fallback)
- **Local CSV Querying**: Parses a 2.5 MB dataset (`dataset/final_restaurants.csv`) containing 29,547 restaurants directly in the browser for instant loading and offline capability.
- **Server API Fallback**: Automatically falls back to a hosted python backend server (`/recommend` endpoint) if client-side loading fails.

---

## 🛠️ Technology Stack

- **Frontend Core:** HTML5, CSS3, ES6+ Javascript
- **Styling Framework:** Tailwind CSS (loaded via CDN)
- **Icons & Typography:** Google Font (Outfit, Inter), Google Material Symbols (Outlined)
- **Hosting & Deployment:** Vercel

---

## 📂 Project Structure

```
FlavourMatch/
├── index.html           # Landing/Home page
├── discover.html        # Main discovery grid with pagination & filters
├── compare.html         # Restaurant comparison panel
├── details.html         # Detailed profile page & recommendations
├── restaurants.js       # Core shared business logic
├── dataset/
│   └── final_restaurants.csv  # Database of 29,547 restaurants
├── images/              # Assets and logos
├── .gitignore           # Git ignore list
└── README.md            # Project documentation
```

---

## 🚀 Running Locally

To run the application locally without any CORS or cross-origin issues with the CSV files, run a local web server in the project directory:

### Python 3:
```bash
python -m http.server 8000
```
Then open your browser and navigate to `http://localhost:8000`.

### Node.js (via http-server):
```bash
npm install -g http-server
http-server -p 8000
```
Then open your browser and navigate to `http://localhost:8000`.

---

## 📄 License

This project is licensed under the MIT License.
