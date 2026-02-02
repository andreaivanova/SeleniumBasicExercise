pipeline {
    agent any
    
    stages{
        stage("restore dependendies"){
           steps{
            bat 'dotnet restore'
           } 
        }

        stage("build the project"){
           steps{
            bat 'dotnet build'
           } 
        }

         stage("run the tests - test 1"){
           steps{
            bat 'dotnet test TestProject1 --no build --verbosity normal'
           } 
        }

          stage("run the tests - test 2"){
           steps{
            bat 'dotnet test TestProject2 --no build --verbosity normal'
           } 
        }

            stage("run the tests - test 3"){
           steps{
            bat 'dotnet test TestProject3 --no build --verbosity normal'
           } 
        }
        }
}
