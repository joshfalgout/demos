pipeline {
    agent { 
        dockerfile true 
        args '-v /root/.m2:/root/.m2'    
    }
    
    
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                docker build . -t "custom:latest" 

            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'node --version'
                sh 'svn --version'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
