pipeline {
    agent any
    stages {
        stage('docker build') {
	 
            steps {
                sh '''
			#sudo systemctl start docker 
   			sudo docker build -f Dockerfile -t test:latest .
		'''
            }
        }     
    }
}
