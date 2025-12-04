# Cypress API Testing

Automated API tests for the Happy Testing application using Cypress.

## Prerequisites

- Node.js 18 or higher
- Backend server running on `http://localhost:3000`

## Installation

```bash
npm install
```

## Running Tests

### Run all API tests
```bash
npm run test:api
```

### Run specific API test suites
```bash
npm run cy:run:api:auth    # Authentication tests
npm run cy:run:api:dishes  # Dishes CRUD tests
npm run cy:run:api:simple  # Simple validation tests
```

### Run tests with Cypress UI
```bash
npm run cy:open
```

### Run tests in headed mode
```bash
npm run test:headed
```

## Project Structure

```
cypress_api_testing/
├── cypress/
│   ├── e2e/
│   │   ├── auth.api.cy.js       # Authentication API tests
│   │   ├── dishes.api.cy.js     # Dishes CRUD API tests
│   │   └── simple.api.cy.js     # Simple validation tests
│   ├── support/
│   │   ├── commands.js          # Custom Cypress commands
│   │   └── e2e.js              # Support file
│   └── fixtures/
│       └── api-test-data.json  # Test data fixtures
├── cypress.config.js           # Cypress configuration
└── package.json

```

## Test Coverage

- **Authentication**: Registration, login, logout
- **Dishes CRUD**: Create, read, update, delete operations
- **Validation**: Data generation, endpoint connectivity
- **Error Handling**: Invalid inputs, missing fields

## CI/CD

Ready to integrate with GitHub Actions or other CI/CD platforms.
