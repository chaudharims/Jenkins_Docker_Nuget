pipeline {
    agent any
    stages {
        stage('docker build') {
            steps {
                sh '''
			systemctl start docker 
   			docker build -f Dockerfile -t test:latest .
		'''
            }
        }     
    }
}
