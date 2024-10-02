# Cherry_Droneshiled - API Tests for PET Endpoint

This repository contains API tests written in Postman for the PET endpoint of a Swagger-based API. The tests are designed to validate various operations (GET, POST, PUT, DELETE) on the PET resource. The tests are integrated with GitHub Actions for Continuous Integration (CI), and the results are automatically generated and viewable in the latest build run.

## Getting Started

### Prerequisites

To run the API tests locally, you will need the following tools installed:

- **Postman**: For API test execution.
- **Newman** (optional): CLI tool to run Postman tests in the terminal.
- **Git**: To clone the repository.
- **Node.js** (if using Newman): To install Newman via npm.

### Installation

1. **Clone the Repository**:
   ```bash
   git clone 
   ```
2. **Navigate to the Branch**:
   Switch to the branch containing the tests:
   ```bash
   git checkout main
   ```

3. **Install Newman (Optional)**:
   If you want to run the tests via Newman (CLI):
   ```bash
   npm install -g newman
   ```

## Running Tests

### Option 1: Run Tests via Postman

1. Open Postman.
2. Import the collection located at `/postman/collections/Pet_Store.json`.
3. Import the environment file located at `/postman/collections/pet_store-env.json`.
4. Run the tests by selecting the collection and clicking **Run**.

### Option 2: Run Tests via Newman (CLI)

1. Run the Postman collection using Newman:
   ```bash
   newman run postman/collections/Pet_Store.json -e postman/collections/pet_store-env.json
   ```

### Option 3: Run Tests via GitHub Actions CI

The tests are automatically run in CI via GitHub Actions on every push or pull request to the repository. You can view the latest test results by navigating to the **Actions** tab in the GitHub repository and reviewing the latest build.

## Viewing Test Reports

After the tests are executed via GitHub Actions, a detailed test report is available in the latest build run. Follow these steps to view the report:

1. Go to the **Actions** tab in the repository.
2. Select the latest workflow run.
3. In the **Run API tests** section, you can view the logs and test results for the PET endpoint API tests.

---

