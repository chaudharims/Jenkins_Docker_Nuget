pipeline {
    agent any
    stages {
        stage('docker build') {
	    agent { 
  			docker { image 'node:14-alpine' } 
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
