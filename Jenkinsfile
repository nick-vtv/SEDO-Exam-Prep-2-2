pipeline{
    agent any
    stages{
        stage("Build .NET Project"){
            steps{
                sh 'dotnet build' // Debian 12
            }
        }
        stage("Test .NET Project"){
            steps{
                sh 'dotnet test --no-build --verbosity normal' // Debian 12
            }
        }
    }
}