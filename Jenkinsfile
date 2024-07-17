pipeline {
    agent any
    stages {
        stage('docker build') {
            steps {
                sh '''
			dockerd --iptables=false
			docker build -f Dockerfile -t test:latest .
		'''
            }
        }     
    }
}
