# Personal Finance Dashboard - Features Specification

## Overview
A comprehensive personal finance dashboard for tracking income, expenses, investments, taxes, and financial projections. This is a frontend-only demo application with interactive functionality using mock data.

---

## 1. Header & Navigation

### Hero Section
- **Description**: Primary welcome area with main value proposition
- **Content**: "Optimize your finances" headline with subtitle "Continuously find money to save and invest"
- **Interaction**: Static display, sets the tone for the application

### Main Navigation
- **Description**: Tab-based navigation between different financial views
- **Tabs**: Accounts, Projections, Cash Flow, Positions, Taxes, Expenses, Action Center
- **Interaction**: Click to switch between different dashboard views

---

## 2. Accounts Management

### Accounts Overview Table
- **Description**: Displays all financial accounts with their types and balances
- **Columns**: Account Name, Type, Balance
- **Account Types**: 
  - Retirement (401k, Roth IRA)
  - Investment (Brokerage)
  - Cash (Savings)
- **Interactions**: 
  - Add new account button
  - Click account to view details
  - Edit account balances (demo mode)
- **Mock Data**: 401k ($250,000), Roth IRA ($75,000), Brokerage ($150,000), Savings ($50,000)

---

## 3. Financial Metrics Dashboard

### Key Metrics Cards
- **Description**: High-level financial overview with key performance indicators
- **Metrics Displayed**:
  - W2 Income: $565,000 (annual)
  - Passive Income: $150,000 (with 44.0% rate indicator)
  - Monthly Expenses: $4,200 (with 44.0% rate indicator)
  - Projected Taxes 2025: $201,000
  - Taxes Withheld 2025: $130,000 (Age 201000 indicator)
  - Current Net Worth: $25,000 (with +12.5% growth)

### Interactions
- **Editable Fields**: Click to modify income and expense values
- **Real-time Updates**: Changes reflect in projections and calculations
- **Tooltips**: Hover for detailed explanations of each metric

---

## 4. Net Worth Projection

### Yearly Projection Chart
- **Description**: Visual representation of projected net worth growth over time (2025-2067)
- **Chart Type**: Bar chart showing yearly progression
- **Y-Axis**: Net worth values ($0 to $3M+)
- **X-Axis**: Years (2025-2067)
- **Interactions**:
  - Hover to see exact values for each year
  - Zoom in/out on time ranges
  - Toggle between different projection scenarios
- **Calculations**: Based on current savings rate, investment returns, and income growth

---

## 5. Cash Flow Management

### Cash Flow Table
- **Description**: Detailed breakdown of income and expense categories with projections
- **Categories**:
  - **Income**: W2 Income, Passive Income (subdivided)
  - **Taxes**: Passive Income Tax, W2 Income Tax, W4 Contributions
  - **Expenses**: Take Home, Redundant expenses
  - **Optimizations**: Tax optimizations, Increase cashflow

### Columns
- Last Year, Last Month, Current Month, Year Projection, Target Monthly Projection, Target Yearly Projection

### Interactions
- **Editable Current Month**: Click to modify current month values
- **Progress Indicators**: Visual bars showing progress toward targets
- **Percentage Calculations**: Automatic calculation of growth rates (+10%, +25%, -15%)
- **Color Coding**: Green for positive trends, red for areas needing attention

---

## 6. Investment Portfolio

### Positions Table
- **Description**: Detailed view of all investment positions and assets
- **Columns**:
  - Portfolio/Asset Name
  - Start Value
  - Contribution (with slider)
  - Withdrawals
  - End Value
  - ROI

### Investment Types
- **401k Traditional**: Vanguard Target Retirement 2065 ($200K → $258K, 29.0% ROI)
- **401k Roth**: Vanguard Target Retirement 2065 ($50K → $58K, 16.0% ROI)
- **After-tax Roth**: Vanguard Total Stock Market ($75K → $95K, 27.0% ROI)
- **IRA**: Vanguard Total International Stock ($100K → $128K, 28.0% ROI)
- **Vulcan**: Vulcan Growth Fund ($150K → $195K, 29.7% ROI)
- **TOD**: Cash ($80K → $102K, 27.0% ROI)
- **Home**: Primary Residence ($500K → $635K, 27.0% ROI)

### Interactions
- **Contribution Sliders**: Adjust monthly contributions for each position
- **Real-time ROI**: Updates based on contribution changes
- **Portfolio Rebalancing**: Suggest optimal allocation
- **Total Portfolio Value**: $1.2M → $1.5M (27.3% overall ROI)

---

## 7. Tax Management

### Tax Breakdown Table
- **Description**: Comprehensive view of all tax obligations and projections
- **Tax Types**:
  - Federal Income Tax: $120K
  - State Income Tax: $45K → $120K current → target $3K (+10%)
  - Social Security Tax: $15K → $120K current → target $15K (0%)
  - Medicare Tax: $9K → $120K current → target $725 (0%)
  - Itemized Deduction: $25K → $2K current → target $2K (0%)

### Columns
- Tax Type, Last Year, Last Month, Current Month, Year Projection, Target Monthly Projection, Target Yearly Projection

### Interactions
- **Tax Strategy Slider**: Adjust withholdings and deductions
- **Optimization Suggestions**: Highlight tax-saving opportunities
- **Scenario Planning**: Compare different tax strategies
- **Total Tax Projection**: $213K → $18K current → $16K target (+8.8%)

---

## 8. Expense Management

### Expense Breakdown
- **Description**: Categorized view of monthly and yearly expenses
- **Categories**:
  - **Housing**: Rent ($24K/year, $2K/month)
  - **Transportation**: Car Payment ($12K/year, $1K/month)
  - **Utilities**: Electricity ($4K/year, $300/month)
  - **Food**: Groceries ($7K/year, $600/month)
  - **Entertainment**: Streaming Services ($1K/year, $100/month)

### Interactions
- **Budget Sliders**: Adjust budgets for each category
- **Expense Tracking**: Add/remove expense categories
- **Spending Analysis**: Compare actual vs budgeted amounts
- **Total Expenses**: $48K/year, $4K/month

---

## 9. Financial Optimization (Action Center)

### Optimization Opportunities
- **Description**: AI-driven suggestions for financial improvements
- **Optimization Types**:
  - **Backdoor Roth IRA**: $7K next month, $78K yearly
  - **Tax-Deferred Account Optimization**: $7K next month, $78K yearly
  - **HSA Tax Benefits**: $4K next month, $46K yearly
  - **Tax Loss Harvesting**: $15K next month, $180K yearly

### Interactions
- **Select Optimization**: Checkboxes to enable/disable optimizations
- **Impact Calculator**: Shows projected savings for each optimization
- **Implementation Guide**: Step-by-step instructions for each optimization
- **Priority Ranking**: Optimizations ranked by potential impact

---

## 10. Data Visualization Components

### Chart Types
- **Bar Charts**: Net worth projection, expense categories
- **Sankey Diagram**: Income flow from sources to investments/expenses
- **Progress Bars**: Goal completion, budget utilization
- **Donut Charts**: Asset allocation, expense distribution
- **Line Charts**: Performance trends over time

### Interactive Features
- **Hover Effects**: Show detailed data on mouse over
- **Zoom/Pan**: Navigate through time ranges
- **Filter Options**: Show/hide specific data series
- **Export Options**: Download charts as images or data

---

## 11. Design System Requirements

### Color Palette
- **Primary**: Blue tones for financial data
- **Success**: Green for positive trends and gains
- **Warning**: Orange for attention areas
- **Danger**: Red for losses or urgent items
- **Neutral**: Grays for backgrounds and text

### Typography
- **Headers**: Clear hierarchy with proper font weights
- **Data**: Monospace fonts for numerical data
- **Body**: Clean, readable sans-serif

### Spacing & Layout
- **Grid System**: Consistent spacing and alignment
- **Card Components**: Modular design for different sections
- **Responsive Breakpoints**: Mobile, tablet, desktop optimization

---

## 12. Interactive Demo Features

### Mock Data Management
- **Realistic Values**: Based on actual financial scenarios
- **State Management**: Changes persist during session
- **Reset Functionality**: Return to default demo values

### User Interactions
- **Form Validation**: Proper input validation and feedback
- **Loading States**: Simulate API calls with loading indicators
- **Success Messages**: Confirmation for user actions
- **Error Handling**: Graceful error states and recovery

### Demo Scenarios
- **Guided Tour**: Walkthrough of key features
- **Sample Calculations**: Pre-filled scenarios showing different financial situations
- **What-if Analysis**: Interactive scenario planning tools

---

## Implementation Priority

### Phase 1 (MVP)
1. Basic layout and navigation
2. Accounts overview
3. Key financial metrics
4. Simple net worth projection

### Phase 2 (Core Features)
1. Cash flow management
2. Investment positions
3. Tax breakdown
4. Expense tracking

### Phase 3 (Advanced Features)
1. Optimization suggestions
2. Advanced visualizations
3. Interactive scenario planning
4. Mobile responsiveness

### Phase 4 (Polish)
1. Animations and micro-interactions
2. Advanced charts and data viz
3. Accessibility improvements
4. Performance optimization