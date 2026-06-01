# Planning & Risks

## Project Overview

| Item          | Value                               |
| ------------- | ----------------------------------- |
| Project       | LifeFlow Fitness                    |
| Developer     | Sofia Andersson                     |
| Course        | 1DV613 Software Development Project |
| Start Date    | 2026-03-30                          |
| End Date      | 2026-06                             |
| Final Version | v1.0.0                              |

---

# Project Scope

## Included in MVP

* User registration and authentication
* Workout logging
* Personal best detection
* Workout templates
* Workout history
* Exercise library
* Dashboard and statistics
* User profile and preferences
* Docker deployment
* CI/CD pipeline
* Documentation and testing

## Excluded from MVP

The following features were intentionally postponed to future versions:

* Calendar and workout planning
* Achievement system
* AI-based recommendations
* Social features
* Native mobile applications
* Payment systems
* Advanced analytics

---

# Development Approach

The project was developed using an iterative and incremental workflow.

Development was divided into multiple iterations, where each iteration focused on a specific set of features.

Each iteration concluded with:

* Completed issues
* Updated documentation
* Testing
* Version tag creation

Version tags were synchronized between frontend and backend repositories.

---

# Iteration Summary

| Version | Focus                                          |
| ------- | ---------------------------------------------- |
| v0.1.0  | Project setup                                  |
| v0.2.0  | Planning and design                            |
| v0.3.0  | Authentication                                 |
| v0.4.0  | Templates and workout history                  |
| v0.5.0  | Docker deployment and feature expansion        |
| v0.6.0  | Dashboard, statistics and quality improvements |
| v0.7.0  | Testing, bug fixing and refinement             |
| v0.8.0  | Final review and documentation                 |
| v1.0.0  | Final delivery                                 |

---

# Risk Management

The following risks were identified during development.

## Risk: Underestimating Development Time

**Likelihood:** High
**Impact:** High

### Mitigation

* Focus on MVP functionality
* Prioritize backlog continuously
* Defer non-essential features

### Outcome

Calendar planning and achievements were postponed to future versions, allowing the MVP to be completed successfully.

---

## Risk: Scope Creep

**Likelihood:** Medium
**Impact:** High

### Mitigation

* Maintain clear MVP boundaries
* Use backlog prioritization
* Separate future features from required functionality

### Outcome

Scope remained manageable throughout the project.

---

## Risk: Complex Workout Data Structures

**Likelihood:** Medium
**Impact:** High

### Mitigation

* Start with a simple domain model
* Refactor incrementally
* Validate using real workout scenarios

### Outcome

The final model successfully supports workouts, templates, exercises, personal bests, and statistics.

---

## Risk: Frontend–Backend Integration Issues

**Likelihood:** Medium
**Impact:** Medium

### Mitigation

* Develop APIs early
* Test endpoints continuously
* Integrate functionality incrementally

### Outcome

No major integration issues occurred.

---

## Risk: Authentication and Security Issues

**Likelihood:** Medium
**Impact:** High

### Mitigation

* Use established libraries
* Validate authentication flows
* Perform both manual and automated testing

### Outcome

JWT authentication and password hashing were implemented successfully.

---

## Risk: Deployment Complexity

**Likelihood:** Medium
**Impact:** High

### Mitigation

* Use Docker containers
* Automate deployment through CI/CD
* Test deployment continuously

### Outcome

The application was successfully deployed and maintained throughout development.

---

# Lessons Learned

The project highlighted the importance of:

* Maintaining a realistic MVP scope
* Prioritizing core functionality before advanced features
* Automating deployment early
* Keeping documentation synchronized with implementation
* Using iterative development to reduce project risk

The most effective decision was to focus on delivering a complete and stable core experience rather than attempting to implement every planned feature.

---

# Final Assessment

The project achieved its primary objectives and delivered a complete MVP that supports:

* Workout tracking
* Progress monitoring
* Personal best detection
* Workout templates
* Statistics and dashboard functionality

Several planned enhancements remain as future work, but all core project goals were successfully completed.
