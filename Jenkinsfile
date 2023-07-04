pipeline {
    agent {
        docker {
            image 'node:16-buster-slim' 
            args '-p 3001:3001' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm cache verify' 
		sh 'npm install'
            } 
		stage('Test') {
            steps {
                sh './jenkins/scripts/test.sh'
            }
        }
        }

    }
}
