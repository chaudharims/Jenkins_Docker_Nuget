pipeline {
    agent any
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
