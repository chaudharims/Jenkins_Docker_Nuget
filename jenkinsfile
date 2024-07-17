pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout your source code from version control
                git 'github.com/chaudharims/nuget.git'
            }
        }     
         
        stage('Pack') {
            steps {
                // Pack your project into a NuGet package
                sh mkdir -p PPP
                sh 'dotnet pack Package.csproj -o PPP --configfile NuGet.Config /p:Version=1.2.3'
            }
        }
        
        stage('Publish') {
            steps {
                // Publish your NuGet package to a NuGet feed
            }
        }
    }
}
