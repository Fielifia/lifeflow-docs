classDiagram

    User "1" --> "*" Workout : owns
    User "1" --> "*" Template : owns
    User "*" --> "*" Exercise : favorites

    Workout *-- WorkoutExercise
    Template *-- TemplateExercise

    WorkoutExercise *-- WorkoutSet
    TemplateExercise *-- TemplateSet


    class User {
        email
        username
        settings
        favorites
    }

    class Workout {
        name
        startTime
        duration
        notes
        personalBests
    }

    class Template {
        name
        notes
    }

    class Exercise {
        name
        target
        bodyPart
        equipment
    }

    class WorkoutExercise {
        exerciseId
        name
        notes
        rest
    }

    class TemplateExercise {
        exerciseId
        name
        notes
        rest
    }

    class WorkoutSet {
        reps
        weight
        completed
        personalBest
    }

    class TemplateSet {
        reps
        weight
    }
