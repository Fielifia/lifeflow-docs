# Testing Strategy

## Overview

LifeFlow Fitness uses a combination of manual testing, automated testing, and exploratory testing.

Testing is requirement-driven, meaning that test cases are derived from functional requirements and user flows. This ensures that implemented functionality is validated against the original project goals.

---

## Traceability

The testing process follows the structure:

```text
User Flow → Requirement → Test Case
```

Examples:

| User Flow               | Requirement                           | Test Cases      |
| ----------------------- | ------------------------------------- | --------------- |
| Register Account        | REQ-1 User Registration               | TC1.1 – TC1.5   |
| User Login              | REQ-2 User Login & Session Management | TC2.1 – TC2.2   |
| Log Workout Session     | REQ-3 Workout Logging                 | TC3.1 – TC3.4   |
| Personal Best Detection | REQ-4 Personal Best Detection         | TC4.1           |
| Workout Templates       | REQ-5 Workout Templates               | TC5.1           |
| Edit Workouts/Templates | REQ-6 Edit Existing Data              | TC6.1           |
| Statistics Overview     | REQ-8 Statistics Overview             | TC8.1           |
| Notes                   | REQ-9 Notes                           | TC9.1           |
| Exercise Library        | REQ-10 Exercise Library               | TC10.1 – TC10.5 |

Calendar Planning (REQ-7) was planned but not implemented in the final release and therefore has no executed test cases.

---

## Test Environment

| Component        | Environment       |
| ---------------- | ----------------- |
| Operating System | Windows 11        |
| Browsers         | Chrome, Firefox   |
| Frontend         | React             |
| Backend          | Node.js / Express |
| Database         | MongoDB           |
| Deployment       | Docker containers |

---

## Testing Approach

### Manual Testing

Manual test cases validate user-facing functionality and API behavior.

Examples include:

* Registration and login
* Workout creation
* Template management
* Statistics retrieval
* Exercise search and filtering

### Automated Testing

Automated tests verify business logic, utility functions, component behavior, and selected end-to-end scenarios.

#### Backend

* Authentication validation
* Workout creation
* Personal best detection
* Statistics calculations

#### Frontend

* Login flow
* Registration flow
* Template state management
* Utility functions

#### End-to-End

* Complete workout flow
* Personal best detection

---

## Security Validation

The following security-related functionality has been verified:

| Security Measure          | Implemented |
| ------------------------- | ----------- |
| Password hashing (bcrypt) | Yes         |
| JWT authentication        | Yes         |
| Token expiration          | Yes         |
| Input validation          | Yes         |
| Authorization middleware  | Yes         |

The application does not currently implement rate limiting or account lockout functionality.

---

## Test Data

A dedicated test account was used during testing.

Email: [test@test.com](mailto:test@test.com)

Password: Password123

The account contains no real user data and can be shared publicly.
