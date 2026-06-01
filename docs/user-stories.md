# User Stories

This document describes the core user stories that defined the scope of the LifeFlow Fitness MVP.

The user stories were used to guide requirements, implementation decisions, and validation throughout development.

Stories marked as planned represent functionality identified for future development beyond the MVP scope.

---

## US-1 — Register Account

**Status:** Implemented

### User Story

As a new user,
I want to register an account,
so that I can save workouts and track progress.

### Acceptance Criteria

* User can register with email and password
* Email must be unique
* Password must be at least 8 characters
* User receives confirmation after successful registration
* User can log in immediately after registration

---

## US-2 — Log In

**Status:** Implemented

### User Story

As a registered user,
I want to log in,
so that I can access my data.

### Acceptance Criteria

* User can log in using email and password
* Invalid credentials show an error message
* Password input is hidden
* User session persists until logout or expiration
* Successful login redirects to the dashboard

---

## US-3 — Log and Track Workout

**Status:** Implemented

### User Story

As a user,
I want to log workouts,
so that I can track my training and progress.

### User Flow

1. User starts a workout session
2. User adds one or more exercises
3. User enters sets, reps, and weight
4. Previous values are automatically pre-filled when available
5. User completes and saves the workout
6. Workout summary is displayed

### Acceptance Criteria

* User can create and complete a workout session
* Exercises can be added, edited, reordered, and removed
* Previous values are automatically pre-filled when available
* Workout data is saved correctly
* Workout summary is displayed after completion

---

## US-4 — Personal Best Tracking

**Status:** Implemented

### User Story

As a user,
I want the system to detect personal bests,
so that I can track my progress.

### User Flow

1. User completes a set
2. System compares the result with previous records
3. If a new record is achieved, it is marked as a personal best
4. Feedback is shown to the user

### Acceptance Criteria

* Personal bests are detected automatically
* Personal bests are visible during and after workouts
* Personal best data is stored correctly

---

## US-5 — Workout Templates

**Status:** Implemented

### User Story

As a user,
I want to create workout templates,
so that I can reuse workout routines.

### User Flow

1. User creates a template
2. User adds exercises and default values
3. Template is saved
4. User starts a workout from the template

### Acceptance Criteria

* Templates can be created
* Templates can be edited
* Templates can be deleted
* Templates can be reused
* Template data is stored correctly

---

## US-6 — Edit Workouts and Templates

**Status:** Implemented

### User Story

As a user,
I want to edit workouts and templates,
so that I can adjust my training records and routines.

### User Flow

1. User opens an existing workout or template
2. User modifies exercises, sets, notes, or values
3. User saves changes
4. System updates the stored data

### Acceptance Criteria

* Existing workouts can be edited
* Existing templates can be edited
* Changes are saved correctly
* Updated data is reflected throughout the application

---

## US-7 — Calendar & Weekly Planning

**Status:** Planned (Future Development)

### User Story

As a user,
I want to plan my workouts,
so that I can follow a structured training routine.

### User Flow

1. User schedules workouts on specific days
2. Calendar displays planned sessions
3. Dashboard displays upcoming workouts

### Acceptance Criteria

* Workouts can be scheduled
* Planned workouts are displayed in a calendar
* Weekly overview is available
* Suggested workouts are displayed appropriately

---

## US-8 — Statistics Overview

**Status:** Implemented

### User Story

As a user,
I want to view my workout statistics,
so that I can understand my progress over time.

### User Flow

1. User opens the statistics page
2. System calculates workout metrics
3. User reviews trends and performance data

### Acceptance Criteria

* Statistics are calculated correctly
* Data updates after completed workouts
* Progress trends are displayed
* Personal best information is available

---

## US-9 — Notes per Exercise or Session

**Status:** Implemented

### User Story

As a user,
I want to add notes to workouts and exercises,
so that I can record important training details.

### User Flow

1. User adds notes during workout creation or editing
2. Notes are saved together with the workout or exercise
3. Notes can be viewed later

### Acceptance Criteria

* Notes can be added and edited
* Notes persist correctly
* Notes are visible in workout details

---

## US-10 — Browse Exercise Library

**Status:** Implemented

### User Story

As a user,
I want to browse and search exercises,
so that I can easily add them to my workouts.

### User Flow

1. User opens the exercise library
2. System displays available exercises
3. User searches by name
4. User filters by muscle group or equipment
5. User browses results
6. User selects an exercise

### Acceptance Criteria

* User can retrieve a list of exercises
* User can search exercises by name
* User can filter exercises by muscle group
* User can filter exercises by equipment
* Results are paginated
* Exercise information includes name, target muscle, equipment, and images

---

## US-11 — Exercise Favorites

**Status:** Implemented

### User Story

As a user,
I want to mark exercises as favorites,
so that I can quickly access frequently used exercises.

### Acceptance Criteria

* Exercises can be marked as favorites
* Favorite exercises are saved per user
* Favorite exercises can be filtered in the exercise library

---

## US-12 — Profile & Settings

**Status:** Partially Implemented

### User Story

As a user,
I want to manage workout preferences,
so that the application better fits my training habits.

### Acceptance Criteria

* User can update monthly workout goals
* User can configure rest timer preferences
* Settings persist between sessions
* User can log out from the settings page

---

## Summary

### Implemented MVP Stories

* US-1 Register Account
* US-2 Log In
* US-3 Log and Track Workout
* US-4 Personal Best Tracking
* US-5 Workout Templates
* US-6 Edit Workouts and Templates
* US-8 Statistics Overview
* US-9 Notes per Exercise or Session
* US-10 Browse Exercise Library
* US-11 Exercise Favorites
* US-12 Profile & Settings

### Planned Future Stories

* US-7 Calendar & Weekly Planning
