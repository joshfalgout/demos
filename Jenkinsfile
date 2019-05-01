pipeline {
    agent { dockerfile true }
    
    
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                args '-v /root/.m2:/root/.m2'

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
