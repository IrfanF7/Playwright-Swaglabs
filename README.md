# 🛒 Swaglabs (Saucedemo) - E2E Test Automation

This repository contains automated End-to-End (E2E) tests for the [Saucedemo](https://www.saucedemo.com/) web application, developed as part of a QA Automation portfolio. The tests are written using **Playwright** and **JavaScript**, demonstrating best practices in UI test automation.

## 🛠️ Tech Stack
- **Framework:** [Playwright](https://playwright.dev/)
- **Language:** JavaScript (Node.js)
- **CI/CD:** GitHub Actions

## 📋 Test Coverage

The automation suite covers the complete user journey, including:

### 1. Authentication
- Valid login
- Invalid login (incorrect username/password)
- Locked out user validation
- Empty fields validation

### 2. Product Catalog
- Product display verification
- Sorting functionality (A-Z, Z-A, Price Low-High, Price High-Low)
- Add/Remove items from the homepage

### 3. Shopping Cart
- Add single and multiple items to the cart
- Verify cart badge counter
- Remove items from the cart page
- "Continue Shopping" navigation

### 4. Checkout Flow
- Positive checkout flow (successful purchase)
- Empty field validations (First Name, Last Name, Postal Code)
- Cancel checkout from the information and overview pages

## 🚀 Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) (v16 or higher)
- npm (Node Package Manager)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/IrfanF7/Playwright-Swaglabs.git
   cd Playwright-Swaglabs
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Install Playwright browsers:
   ```bash
   npx playwright install
   ```

### 🏃 Running Tests

Run all tests in headless mode:
```bash
npx playwright test
```

Run tests with UI mode:
```bash
npx playwright test --ui
```

Run tests in a specific browser (e.g., Chromium):
```bash
npx playwright test --project=chromium
```

View the detailed HTML report after test execution:
```bash
npx playwright show-report
```

## 📁 Project Structure

```text
├── .github/workflows/      # GitHub Actions CI/CD pipeline configuration
├── tests/                  # Playwright test scripts (*.spec.js)
│   ├── Cart.spec.js
│   ├── Checkout.spec.js
│   ├── Homepage.spec.js
│   └── Login.spec.js
├── package.json            # Project dependencies and scripts
├── playwright.config.js    # Playwright configuration file
└── README.md               # Project documentation
```

## ⚙️ Continuous Integration (CI/CD)
This project is integrated with **GitHub Actions**. Every push to the `main` branch triggers an automated workflow that:
- Sets up the Node.js environment
- Installs dependencies and Playwright browsers
- Executes the entire test suite
- Uploads the Playwright HTML report as an artifact

---
*Created by [Irfan](https://github.com/IrfanF7) - QA Engineer*
