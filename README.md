# Tech Quiz Test Suite

![MIT License](https://img.shields.io/badge/License-MIT-yellow.svg)

## Description

**Tech Quiz Test Suite** is a testing suite designed for the Tech Quiz application, ensuring its functionality, reliability, and user experience through rigorous testing. Utilizing both **End-to-End (E2E)** and **Component** testing methodologies with Cypress, this suite verifies every aspect of the quiz lifecycle—from initiating the quiz, answering questions, to viewing final scores.

**Key Features:**

- **End-to-End Testing:** Simulates real user interactions to validate the entire application flow.
- **Component Testing:** Tests individual components in isolation to ensure they function as intended.

## Table of Contents 

- [Installation](#installation)
- [Usage](#usage)
- [Credits](#credits)
- [License](#license)
- [Contributing](#contributing)
- [Tests](#tests)
- [Questions](#questions)

## Installation

To set up and run the Tech Quiz application along with its E2E test suite in development mode, follow these steps:

1. **Clone the Repository:**
    ```bash
    git clone git@github.com:Connorldailey/Tech-Quiz-Test-Suite.git
    ```

2. **Navigate to the Project Directory:**
    ```bash
    cd Tech-Quiz-Test-Suite
    ```

3. **Install Dependencies:**
    ```bash
    npm install
    ```

4. **Set Up Environment Variables:**
    - Create a `.env` file in the `server` directory.
    - Use the `.env.example` file as a template, filling in the necessary values.
    
    ```bash
    cp server/.env.example server/.env
    ```

5. **Build the Application:**
    ```bash
    npm run build
    ```

6. **Seed the Database:**
    ```bash
    npm run seed
    ```

7. **Launch the Application:**
    ```bash
    npm run start:dev
    ```

8. **Open Cypress Test Runner:**
    ```bash
    npm run cypress
    ```
    - This will launch the Cypress Test Runner interface where you can run the tests interactively.


## Usage

Below are steps for using the Tech Quiz and running its tests:

1. **Access the Application**  
   - Open `http://localhost:3000` (or your chosen port) to use the Tech Quiz.

2. **Running Tests**  
   - **Interactive Mode:**  
     ```bash
     npm run cypress:open
     ```  
     - In the Cypress Test Runner, select **E2E** (e.g., `quiz.cy.js`) or **Component** tests (e.g., `Quiz.cy.jsx`).
   - **Headless Mode:**  
     ```bash
     npm run test
     ```  
     - Executes all tests (E2E and Component) in headless mode.

3. **Review Test Results**  
   - Cypress offers logs, screenshots, and videos (if enabled) for debugging and analysis.

[Walkthrough Video](https://drive.google.com/file/d/1j9zRzsnNbyAZkQO40hXVCHJLJu15_912/view?usp=sharing)

## Credits

- **Application Provided By:** The Ohio State University Coding Bootcamp
- **Tests Written By:** [Connor Dailey](https://github.com/connorldailey)

## License

This project is licensed under the MIT License - see the [MIT License](https://opensource.org/licenses/MIT) for details. 

## Contributing

Contributions are currently not being accepted. Thank you for your interest!

## Tests

This application includes an automated test suite using Cypress for comprehensive coverage. Both End-to-End (E2E) and Component tests are provided.

### Test Types

- **E2E Tests** (`cypress/e2e/quiz.cy.js`)  
  Validates full user flows, including starting quizzes, answering questions, and viewing final results.

- **Component Tests** (`cypress/component/Quiz.cy.jsx`)  
  Focus on individual React components (e.g., `<Quiz />`), ensuring proper rendering, state management, and interactions.

### Scripts

- **npm run cypress**  
  Opens the Cypress Test Runner for interactive E2E and Component tests.

- **npm run cypress:open**  
  Runs the development server and opens the Cypress Test Runner simultaneously.

- **npm run test**  
  Executes all Cypress tests in headless mode.

**Note:** The server must be running to perform tests.

### Scenarios

1. **E2E**  
   - Loads the quiz page, starts the quiz, and verifies question flow.  
   - Checks score updates and final quiz completion screen.

2. **Component**  
   - Renders `<Quiz />` with a "Start Quiz" button.  
   - Ensures proper state updates when selecting answers.  
   - Verifies correct score display and quiz restart functionality.

## Questions

If you have any questions about this project, feel free to reach out: 

- **GitHub:** [connorldailey](https://github.com/connorldailey)
- **Email:** connorldailey@gmail.com