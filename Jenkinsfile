pipeline {
    agent any
    stages {
        stage('docker build') {
            steps {
                sh '''
			sudo dockerd --iptables=false
			docker build -f Dockerfile -t test:latest .
		'''
            }
        }     
    }
}
