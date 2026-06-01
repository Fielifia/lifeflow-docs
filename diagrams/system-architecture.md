flowchart LR

    User([User])

    subgraph Frontend["React Frontend"]
        Dashboard
        WorkoutFlow["Workout Tracking"]
        Templates
        History
        Statistics
        Profile
        ExerciseLibrary["Exercise Library"]
    end

    subgraph Backend["Node.js / Express API"]
        Auth["Authentication"]
        WorkoutAPI["Workout Services"]
        TemplateAPI["Template Services"]
        StatsAPI["Statistics Services"]
        UserAPI["User Services"]
        ExerciseAPI["Exercise Services"]
    end

    DB[(MongoDB)]

    User --> Dashboard
    User --> WorkoutFlow
    User --> Templates
    User --> History
    User --> Statistics
    User --> Profile
    User --> ExerciseLibrary

    Dashboard --> Backend
    WorkoutFlow --> Backend
    Templates --> Backend
    History --> Backend
    Statistics --> Backend
    Profile --> Backend
    ExerciseLibrary --> Backend

    Backend --> DB
