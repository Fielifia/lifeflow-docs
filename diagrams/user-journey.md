flowchart TD

    Login[Register / Login]

    Login --> Dashboard

    Dashboard --> StartWorkout
    Dashboard --> Templates
    Dashboard --> History
    Dashboard --> Statistics
    Dashboard --> ExerciseLibrary
    Dashboard --> Profile

    %% Workout flow

    StartWorkout --> EmptyWorkout[Start Empty Workout]
    StartWorkout --> TemplateWorkout[Start From Template]

    %% Template flow

    Templates --> CreateTemplate[Create Template]
    Templates --> EditTemplate[Edit Template]
    Templates --> TemplateWorkout

    %% Exercise Library

    ExerciseLibrary --> SearchExercises[Search & Filter Exercises]
    SearchExercises --> FavoriteExercise[Mark Favorite Exercise]

    %% Workout

    EmptyWorkout --> AddExercises
    TemplateWorkout --> AddExercises

    AddExercises --> LogSets

    LogSets --> PB{New Personal Best?}

    PB -->|Yes| ShowPB[Display Personal Best]
    PB -->|No| SaveWorkout

    ShowPB --> SaveWorkout

    %% History

    SaveWorkout --> History

    History --> ViewWorkout[View Workout]
    ViewWorkout --> EditWorkout[Edit Workout]

    %% Statistics

    Statistics --> ProgressTracking[View Progress Statistics]

    %% Profile

    Profile --> Settings[Manage Goals & Preferences]
