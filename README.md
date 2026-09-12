# Aura Finance

**A simple web app to track money, plan budgets, and get AI-based spending advice.**

Live Demo: https://aura-financ.web.app

<video src="assets/demo.mp4" controls width="100%"></video>

Aura Finance helps you see where your money goes. Add your income and expenses, set monthly limits, create savings goals, and ask an AI assistant questions about your spending. Your data is private to your account and updates instantly on all devices.

### Who is this for?

* **Non-technical users:** Anyone who wants an easy way to manage personal money.
* **Recruiters / Reviewers:** A complete full-stack project showing React, Firebase, and AI integration.
* **Students / Freshers:** A clean example to learn auth, database, and real-time data in React.

## What you can do

* **See all money in one place:** Dashboard with balance, income, expenses, and monthly charts.
* **Add transactions:** Record income/expenses with search, filters, and categories.
* **Set budgets:** Monthly limits per category with progress bars and overspending alerts.
* **Track savings goals:** Create goals (e.g. vacation), add savings, see progress.
* **Ask AI for help:** Chat assistant that looks at your actual data to give saving tips.
* **Use your currency:** Switch between USD, EUR, GBP, INR, JPY.
* **Login securely:** Email/password + Google login. Each user only sees their own data.

## How it works (simple flow)

1. You sign up / log in.
2. You add transactions, budgets, and goals — saved securely in Firebase.
3. Dashboard, notifications, and AI use that data to show insights.

No need to read the code to understand it — this is the full idea.

## Tech used

| Tech | Used for |
|---|---|
| React + TypeScript + Vite | App interface and fast development |
| Tailwind CSS | Styling |
| Firebase Auth + Firestore | Login and secure cloud database |
| Google Gemini API | AI chat insights |
| Finnhub API (optional) | Market prices, else shows demo data |

Full technical details are in `DEVELOPMENT.md`. Interview Q&A is in `INTERVIEW_PREP.md`.

## Run it locally

1. Clone:
   ```bash
   git clone https://github.com/mohaktalodhikar/aura-finance.git
   ```
2. Install:
   ```bash
   npm install
   ```
3. Create a `.env` file with your keys:
   ```env
   VITE_FIREBASE_API_KEY=your-key
   VITE_FIREBASE_AUTH_DOMAIN=your-project.firebaseapp.com
   VITE_FIREBASE_PROJECT_ID=your-project-id
   VITE_FIREBASE_STORAGE_BUCKET=your-project.appspot.com
   VITE_FIREBASE_MESSAGING_SENDER_ID=your-id
   VITE_FIREBASE_APP_ID=your-id
   VITE_GEMINI_API_KEY=your-gemini-key
   VITE_FINNHUB_API_KEY=your-finnhub-key
   ```
   > Gemini and Finnhub keys are optional — app works without them.

4. Start:
   ```bash
   npm run dev
   ```

To get Firebase keys: Firebase Console > Create Project > Enable Auth (Email + Google) + Firestore > Copy web config.

## Project structure (short)

```
src/
  App.tsx          # Login check + page switching
  firebase.ts      # Firebase setup
  context/         # Shared data (transactions, budgets, goals)
  components/      # Sidebar, TopNav, BottomNav
  views/           # Login, Overview, Transactions, Budgets, Insights, Settings
```

## About the developer

**Mohak Talodhikar**

- [LinkedIn](https://www.linkedin.com/in/mohak-talodhikar/)
- [GitHub](https://github.com/mohaktalodhikar)
- [Instagram](https://www.instagram.com/mohak_talodhikar/)