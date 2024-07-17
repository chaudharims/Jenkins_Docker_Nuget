pipeline {
    agent any
    triggers {
        // Trigger on changes in the Git repository
    }
    stages {
        stage('docker build') {
            steps {
                sh '''
			docker build -f Dockerfile -t test:latest .
		'''
            }
        }     
    }
}
