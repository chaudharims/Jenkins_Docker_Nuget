pipeline {
    agent any
    stages {
        stage('docker build') {
            steps {
                sh '''
			export DOCKER_HOST=unix:///run/user/$(id -u)/docker.sock 
   			docker build -f Dockerfile -t test:latest .
		'''
            }
        }     
    }
}
