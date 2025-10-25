pipeline{
    agent any

    stages{        
        stage("Build application"){
            steps{
                bat 'dotnet build' // For Windows (according to exam requirements - no separate restore stage)
            }
        }
        stage("Run unit and integration tests"){
            steps{
                bat 'dotnet test --no-build --verbosity normal'
            }
        }
    }
}
