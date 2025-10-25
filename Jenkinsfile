pipeline{
    agent any
    stages{
        stage("Restore .NET Dependencies"){
            steps{
                sh 'dotnet restore'
            }
        }
        stage("Build .NET Project"){
            steps{
                sh 'dotnet build --no-restore'
            }
        }
        stage("Test .NET Project"){
            steps{
                sh 'dotnet test --no-build --verbosity normal'
            }
        }
    }
}