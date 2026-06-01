# Manual Test Cases

## Overview

The following manual test cases were executed to verify that the implemented requirements work as expected.

Each test case is linked to a functional requirement and derived from the corresponding user flow.

---

# REQ-1 User Registration

## TC1.1 Successful Registration

**Requirement:** REQ-1

### Steps

1. Open the registration page.
2. Enter a valid email address.
3. Enter a username.
4. Enter a password with at least 8 characters.
5. Submit the form.

### Expected Result

* Account is created successfully.
* User is authenticated.
* User is redirected into the application.

---

## TC1.2 Duplicate Email Rejected

**Requirement:** REQ-1

### Steps

1. Register a user.
2. Attempt to register another user using the same email address.

### Expected Result

* Registration is rejected.
* Appropriate error message is displayed.

---

## TC1.3 Password Too Short

**Requirement:** REQ-1

### Steps

1. Open registration form.
2. Enter a password shorter than 8 characters.
3. Submit the form.

### Expected Result

* Registration is rejected.
* Validation error is displayed.

---

## TC1.4 Missing Required Fields

**Requirement:** REQ-1

### Steps

1. Leave one or more required fields empty.
2. Submit the form.

### Expected Result

* Registration is rejected.
* Validation error is displayed.

---

## TC1.5 Email Normalization

**Requirement:** REQ-1

### Steps

1. Register using uppercase letters and surrounding spaces in the email address.

### Expected Result

* Email is normalized and stored correctly.

---

# REQ-2 User Login & Session Management

## TC2.1 Successful Login

**Requirement:** REQ-2

### Steps

1. Open login page.
2. Enter valid credentials.
3. Submit login form.

### Expected Result

* Login succeeds.
* User is redirected to the dashboard.

---

## TC2.2 Invalid Credentials

**Requirement:** REQ-2

### Steps

1. Enter invalid credentials.
2. Submit login form.

### Expected Result

* Login is rejected.
* Error message is displayed.

---

# REQ-3 Workout Logging

## TC3.1 Successful Workout Logging

**Requirement:** REQ-3

### Steps

1. Start a new workout.
2. Add one or more exercises.
3. Add sets, reps, and weight.
4. Save workout.

### Expected Result

* Workout is stored successfully.
* Workout appears in history.

---

## TC3.2 Minimal Workout Logging

**Requirement:** REQ-3

### Steps

1. Start a workout.
2. Enter only required information.
3. Save workout.

### Expected Result

* Workout can be completed successfully.

---

## TC3.3 Missing Workout Name

**Requirement:** REQ-3

### Steps

1. Create workout without a name.
2. Attempt to save.

### Expected Result

* Save is rejected.
* Validation error is displayed.

---

## TC3.4 Unauthorized Workout Creation

**Requirement:** REQ-3

### Steps

1. Attempt to create a workout without authentication.

### Expected Result

* Request is rejected.

---

# REQ-4 Personal Best Detection

## TC4.1 Personal Best Detected

**Requirement:** REQ-4

### Steps

1. Log a workout containing a better result than a previous workout.
2. Save workout.

### Expected Result

* Personal best is detected automatically.
* Personal best indicator is displayed.

---

# REQ-5 Workout Templates

## TC5.1 Template Creation

**Requirement:** REQ-5

### Steps

1. Create a new workout template.
2. Add exercises.
3. Save template.

### Expected Result

* Template is stored successfully.
* Template can be reused later.

---

# REQ-6 Edit Workouts and Templates

## TC6.1 Edit Existing Workout or Template

**Requirement:** REQ-6

### Steps

1. Open an existing workout or template.
2. Modify exercises or values.
3. Save changes.

### Expected Result

* Changes are saved correctly.
* Updated data is displayed.

---

# REQ-8 Statistics Overview

## TC8.1 View Statistics

**Requirement:** REQ-8

### Steps

1. Complete several workouts.
2. Open statistics page.

### Expected Result

* Statistics are displayed correctly.
* Workout counts and volume calculations appear reasonable.

---

# REQ-9 Notes

## TC9.1 Add Notes

**Requirement:** REQ-9

### Steps

1. Open workout creation or editing.
2. Add notes.
3. Save workout.

### Expected Result

* Notes are stored successfully.
* Notes remain visible when viewing the workout later.

---

# REQ-10 Exercise Library

## TC10.1 Retrieve Exercises

**Requirement:** REQ-10

### Steps

1. Open Exercise Library.

### Expected Result

* Exercise list is displayed.

---

## TC10.2 Search Exercises

**Requirement:** REQ-10

### Steps

1. Search for an exercise by name.

### Expected Result

* Matching exercises are displayed.

---

## TC10.3 Filter by Muscle Group

**Requirement:** REQ-10

### Steps

1. Select a muscle group filter.

### Expected Result

* Matching exercises are displayed.

---

## TC10.4 Filter by Equipment

**Requirement:** REQ-10

### Steps

1. Select an equipment filter.

### Expected Result

* Matching exercises are displayed.

---

## TC10.5 Pagination

**Requirement:** REQ-10

### Steps

1. Navigate through exercise pages.

### Expected Result

* Different exercise results are displayed for each page.
