pipeline {
    agent any
    stages {
        stage('docker build') {
	   agent {
                docker { image 'node:20.15.1-alpine3.20' }
		args '-u root'
		reuseNode true
            }
            steps {
                sh '''
			sudo systemctl start docker 
   			docker build -f Dockerfile -t test:latest .
		'''
            }
        }     
    }
}
