FINTRACK – Personal Finance Manager for Students

Know your money. Control your spending. Reach your goals.

FINTRACK is a web application that helps college students understand where their money goes, stay within a budget, and save for goals. It is built with plain HTML, CSS and JavaScript, so it needs no backend and no installation.

Live demo: https://fin-track-eight-neon.vercel.app/

Problem Statement

Many college students receive a fixed monthly allowance but have no simple way to see where it goes. Small daily expenses add up, money runs out before the month ends, and saving rarely happens. Most finance apps are designed for working adults and are too complex for students.

Objectives
Make it easy to record daily expenses by category and payment method
Help students set and follow monthly budgets
Show spending patterns through clear charts and reports
Support savings goals with a realistic timeline
Give one simple daily spending limit through the Safe to Spend calculator
Features
Module	What it does
Safe to Spend	Calculates a daily limit: (monthly money − spent − planned expenses) ÷ days left in the month
Expense Tracker	Add, edit and delete expenses with amount, category, date and payment method (UPI, Cash, Card)
Budget Planner	Set monthly limits per category with progress bars (amber at 80%, red when exceeded)
Budget Alerts	Warnings such as "You've used 85% of your Food & Canteen budget"
Spending Analytics	Category donut chart and weekly spending bar chart (Chart.js)
Savings Goals	Track progress toward goals and estimate months remaining
Monthly Report	Totals, comparison with last month, and simple insights
3D Landing Page	Scroll-driven 3D intro built with Three.js, with a live Safe to Spend demo
Tech Stack
HTML5 for structure
CSS3 for the responsive dark interface
JavaScript (ES6) for calculations and application logic
localStorage for saving data in the browser
Chart.js for charts
Three.js for the 3D landing page
Project Structure
fintrack/
├── index.html      # 3D landing page (opens first)
├── fintrack.html   # The finance app
└── README.md
How to Run Locally
Download or clone this repository.
Keep index.html and fintrack.html in the same folder.
Open index.html in a browser and click Open app.

An internet connection is needed for the fonts, Chart.js and Three.js, which load from CDNs.

Deployment

This is a static site, so it can be hosted free on Vercel, GitHub Pages or Netlify. On Vercel: import the repository, set the framework preset to Other, leave the build settings empty, and click Deploy.

How the Safe to Spend Calculation Works

Example: a student starts the month with ₹6,000, has spent ₹2,000, has ₹1,000 of planned expenses and has 20 days left.

(6000 − 2000 − 1000) ÷ 20 = ₹150 per day

This is a budgeting estimate, not a financial guarantee.

Limitations
Data is stored only in the browser, so it is not shared between devices and is lost if browser data is cleared
There are no user accounts
Expenses must be entered manually
Future Scope
User accounts and cloud sync (Firebase or Node.js backend)
Automatic expense import from UPI and SMS
AI-based spending insights and predictions
Bill and subscription reminders
Recurring expenses
Installable mobile version (PWA)
Bill splitting between friends
Disclaimer

FINTRACK is a budgeting aid built for learning. It does not provide financial advice.

Author
Sushant Yadav
