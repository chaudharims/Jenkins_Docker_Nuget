pipeline {
    agent any
    triggers { always: true }
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
