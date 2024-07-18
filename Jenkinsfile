pipeline {
    agent any
    stages {
        stage('docker build') {
	   agent {
                docker { image 'node:20.15.1-alpine3.20' }
            }
            steps {
                sh '''
			systemctl start docker 
   			docker build -f Dockerfile -t test:latest .
		'''
            }
        }     
    }
}
