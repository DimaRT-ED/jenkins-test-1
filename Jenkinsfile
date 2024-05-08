pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                sh 'ls -la'
                echo 'Build finished....'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'cat README.md'
                echo 'Test finished....'
            }
        }   
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                sh 'ls -la'
                echo 'Deploy finished....'
            }
        }
    }  
    post {
        success {
            echo 'Pipeline succeeded!  HO-HO-HO !!! FROM NEW BRANCH'
        }
        failure {
            echo 'Pipeline failed!   HO-HO-HO !!! FROM NEW-BRANCH '
        }
    }
}
