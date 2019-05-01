pipeline {
    agent { dockerfile {-id} }
    
    
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'ls'

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
