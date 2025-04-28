Personal Finance Visualizer

A comprehensive web application for tracking, managing, and visualizing personal finances, including transactions, budgeting, and financial insights.

Features:
   Transaction Management: Add, edit, and delete financial transactions with categorization
   Financial Dashboard: View key metrics and visualizations of your spending patterns
   Budgeting Tools: Set and track budgets by category and month
   Interactive Charts: Visualize spending trends and budget comparisons
   Responsive Design: Works on desktop and mobile devices

Frontend:
   React.js
   Recharts for data visualization
   CSS for styling
   Backend
Node.js:
   Express.js
   MongoDB for data storage
   RESTful API architecture

API Endpoints

Transactions:
      GET /api/transactions - Get all transactions
      GET /api/transactions/:id - Get a single transaction
      POST /api/transactions - Create a new transaction
      PUT /api/transactions/:id - Update a transaction
      DELETE /api/transactions/:id - Delete a transaction
Categories:
      GET /api/categories - Get all categories
      POST /api/categories - Create a new category
      DELETE /api/categories/:id - Delete a category
Budgets:
      GET /api/budgets - Get all budgets
      GET /api/budgets/:id - Get a single budget
      POST /api/budgets - Create a new budget
      PUT /api/budgets/:id - Update a budget
      DELETE /api/budgets/:id - Delete a budget

Data Models
{
  _id: ObjectId,
  amount: Number,
  date: Date,
  description: String,
  category: String
}
Category
{
  _id: ObjectId,
  name: String
}
Budget
{
  _id: ObjectId,
  category: String,
  amount: Number,
  month: String // Format: "YYYY-MM"
}
Usage

Adding Transactions

  1. Navigate to the "Transactions" tab
  2. Fill out the transaction form with amount, date, description, and category
  3. Click "Add Transaction"
  4. 
Setting Budgets

  1. Navigate to the "Budgeting" tab
  2. Select a category and month
  3. Enter your budget amount
  4. Click "Set Budget"

Viewing Financial Insights

  1. Navigate to the "Dashboard" tab to see your spending breakdown
  2. Check the "Monthly Expenses" chart to track spending over time
  3. Use the "Budget vs. Actual Spending" chart to monitor your budget adherence

Acknowledgements
   React
   Express
   MongoDB
   Recharts









