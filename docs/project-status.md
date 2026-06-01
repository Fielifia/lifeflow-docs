# Project Status

## Overview

LifeFlow Fitness is a fullstack fitness tracking application developed as part of the 1DV613 Software Development Project course.

The application allows users to register accounts, track workouts, manage workout templates, browse exercises, review workout history, and analyze training progress through statistics and dashboard views.

The project has been developed using an iterative and agile workflow with continuous requirements management, testing, versioning, and deployment.

---

# Current Development Status

The project is currently in the **final delivery phase**.

Core MVP functionality has been implemented, tested, documented, and deployed.

Remaining work primarily consists of future improvements rather than unfinished MVP requirements.

---

# Implemented Functionality

## Authentication

Implemented:

* User registration
* User login
* JWT-based authentication
* Password hashing using bcrypt
* Protected API routes

---

## Exercise Library

Implemented:

* Browse exercises
* Search exercises by name
* Filter by muscle group
* Filter by equipment
* Pagination
* Favorite exercises

---

## Workout Logging

Implemented:

* Create workout sessions
* Add exercises
* Add sets, reps, and weight
* Exercise notes
* Rest timer support
* Workout duration tracking
* Previous value suggestions
* Active workout management
* Discard workout functionality

---

## Personal Best Detection

Implemented:

* Automatic personal best detection
* Personal best indicators
* Personal best statistics

---

## Workout Templates

Implemented:

* Create templates
* Edit templates
* Delete templates
* Start workouts from templates

---

## Workout History

Implemented:

* Workout overview
* Detailed workout views
* Edit completed workouts
* Delete workouts
* Start new workouts from previous sessions

---

## Statistics & Dashboard

Implemented:

* Workout frequency statistics
* Total volume calculations
* Exercise usage statistics
* Personal best statistics
* Monthly goal tracking
* Recent workout activity
* Dashboard summaries

---

## Profile & Settings

Implemented:

* Monthly workout goals
* Default rest timer settings
* Rest timer preferences
* Sound preferences
* User profile information
* Logout functionality

---

## Infrastructure

Implemented:

* React frontend
* Node.js / Express backend
* MongoDB database
* Docker deployment
* Docker Compose
* nginx reverse proxy
* HTTPS support
* GitLab CI/CD pipelines
* Semantic versioning

---

# Remaining Work

The MVP is considered complete.

The following items remain as future improvements:

* Calendar and workout planning
* Achievement system
* Expanded automated test coverage
* Advanced statistics and visualizations
* Additional profile customization
* Progressive Web App (PWA) support
* AI-assisted workout recommendations

These features were intentionally deferred to maintain focus on the MVP scope.

---

# Testing Status

Testing has been performed using a combination of manual and automated testing.

## Manual Testing

Manual test cases were executed for:

* User registration
* User login
* Workout logging
* Personal best detection
* Workout templates
* Workout editing
* Statistics
* Notes
* Exercise library

### Results

| Result | Count |
| ------ | ----- |
| Passed | 19    |
| Failed | 0     |

REQ-7 (Calendar Planning) was not implemented and therefore has no executed test cases.

---

## Automated Testing

Implemented automated tests include:

### Backend

* Authentication validation
* Workout validation
* Personal best calculations
* Statistics calculations

### Frontend

* Login flow
* Registration flow
* Application rendering
* Utility functions
* Template management

### End-to-End

* Complete workout flow
* Personal best detection

Automated tests are executed through the CI/CD pipeline.

---

# Project Outcome

The project successfully achieved its primary objective:

> To create a simple and efficient fitness tracking application focused on workout logging, progress tracking, and user motivation.

The delivered MVP provides a complete workflow from account creation to workout tracking, historical analysis, and progress monitoring while maintaining a simple and user-friendly experience.
