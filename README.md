#  Crypto Portfolio Tracker

A full-stack web application that allows users to manage, monitor, and track their cryptocurrency investments in real-time. The application provides secure login functionality, live market price updates, and a clean, interactive dashboard for portfolio management.
This project was built during my internship to demonstrate full-stack development skills, integration of real-time APIs, and the ability to design scalable systems from scratch.

---
Overview
Cryptocurrency investors often need a centralized, live, and user-friendly tool to manage their holdings. This tracker allows users to:
- Add various crypto assets to their personal portfolio
- Monitor the real-time value of those assets
- Calculate total portfolio value based on market fluctuations
- View intuitive and responsive dashboards
- 
---
Features
- Secure User Authentication 
  Using JWT tokens for stateless and protected user access
- Real-Time Crypto Price Tracking 
  Integrated with APIs like CoinGecko to fetch live market prices
- Portfolio Management
  Add, update, or remove crypto assets to simulate your investments
- Interactive Dashboard
  View dynamic updates to asset value and portfolio performance
- Frontend-Backend Sync
  Smooth RESTful communication between Flask and React

---
Tech Stack
| Layer       | Technology                        |
|-------------|-----------------------------------|
| Frontend    | React, JavaScript, Axios          |
| Backend     | Python, Flask, REST APIs          |
| Auth        | JWT (JSON Web Tokens)             |
| API Source  | CoinGecko / CoinMarketCap         |
| Tools       | Postman, Git, VS Code, Node.js    |

---
Project Structure
```
crypto\_portfolio\_tracker/
├── run.py                     # Entry point for Flask backend
├── requirements.txt           # Backend dependencies
├── backend/
│   ├── **init**.py            # Flask app setup
│   ├── routes.py              # Auth and portfolio endpoints
│   ├── models.py              # User and asset data models
│   └── utils.py               # API handlers and helpers
├── frontend/
│   ├── package.json           # Frontend dependencies
│   ├── public/                # Static files
│   └── src/                   # React components

````

---
Getting Started
Backend Setup
1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/crypto-portfolio-tracker.git
    cd crypto_portfolio_tracker
    ```

2. Create and activate virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate  # Linux/macOS
    venv\Scripts\activate     # Windows
    ```

3. Install Python dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Run the Flask server:
    ```bash
    python run.py
    ```

Frontend Setup
1. Navigate to frontend directory:
    ```bash
    cd frontend
    ```

2. Install frontend dependencies:
    ```bash
    npm install
    ```

3. Start the frontend server:
    ```bash
    npm start
    ```

---
API Endpoints (Backend)
| Method | Endpoint          | Description                          |
|--------|-------------------|--------------------------------------|
| POST   | `/register`       | Create a new user                    |
| POST   | `/login`          | Authenticate user and return JWT     |
| GET    | `/portfolio`      | Get user's portfolio (JWT required)  |
| POST   | `/portfolio`      | Add asset to portfolio               |
| DELETE | `/portfolio/<id>` | Remove asset from portfolio          |

---
What I Learned
- Full-stack development using Flask and React
- API integration with real-time data
- Token-based authentication and session security
- Building scalable, modular web architectures
- Handling asynchronous data and frontend-backend sync
- Debugging complex data flows and managing component state

---
Challenges Faced
| Challenge                             | Solution                                                                 |
|--------------------------------------|--------------------------------------------------------------------------|
| Real-time API rate limits            | Added retry logic and basic caching to reduce external API dependency    |
| User session and authentication      | Implemented secure JWT token system for authentication                   |
| Data sync between frontend/backend   | Used consistent REST schema and Axios with error handling                |
| Portfolio state updates              | Optimized React component updates with `useEffect()` and state hooks     |

---
Future Enhancements
- Wallet address auto-sync (via blockchain APIs)
- Charting portfolio trends using Chart.js or Recharts
- Push notifications for price alerts
- Enhanced admin dashboard
- Deployment via Docker or cloud hosting (e.g., Vercel/Render)

---
Contributing
Contributions, suggestions, and improvements are welcome!  
Please open an issue or submit a pull request.

---
 License
This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

---
Developer
Priyanshu Tonk
📌 Passionate about full-stack development, crypto tech, and real-time applications  
🔗 [LinkedIn](https://www.linkedin.com/in/priyanshu-in002004/)  
📧 Email: priyanshutonk.in@gmail.com
