🚀 Crypto Dashboard
A full-stack MERN application that fetches crypto market data from CoinGecko, stores historical snapshots, and displays data beautifully with React and Tailwind CSS.

💻 Tech Stack
Frontend:

React (Vite)

Tailwind CSS

Axios

React Router DOM

Backend:

Node.js

Express.js

Mongoose (MongoDB)

Node-Cron

dotenv

cors

Database:

MongoDB (Atlas or local)

⚙️ Setup & Installation
1. Clone the repo
bash
Copy
Edit
git clone https://github.com/Riya-JAIN2001/vr_Automation_test.git
cd your-repo
2. Backend Setup
bash
Copy
Edit
cd backend
npm install
Create a .env file in the backend folder:

ini
Copy
Edit
PORT=5000
MONGO_URI=your_mongodb_connection_string
Start the backend:

bash
Copy
Edit
npm start
3. Frontend Setup
bash
Copy
Edit
cd frontend
npm install
npm run dev
The frontend will run locally (usually at http://localhost:5173).

⏰ How the Cron Job Works
Scheduled to run every 30 minutes using node-cron.

Fetches the top 10 crypto coins from the CoinGecko API.

Saves the fetched data into the History collection in MongoDB (instead of updating the Coins collection).

Data stored includes:

coinId

name

image

price

marketCap

change24h

lastUpdated

snapshotTime

This enables tracking and analysis of historical crypto trends over time.

🌐 Deployed Links
Frontend : https://vr-automation-frontend.vercel.app/

Backend : https://vr-backend-kyc2.onrender.com

API Example
bash
Copy
Edit
GET /api/history
Returns all snapshots of crypto market data.

Tailwind CSS
This project uses Tailwind CSS for styling. Configuration is in:

bash
Copy
Edit
frontend/tailwind.config.js
frontend/src/index.css
