pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building the project...  FROM -- OTHER -- BRANCH'
                sh 'ls -la'
                echo 'Build finished....'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests... FROM -- OTHER -- BRANCH'
                sh 'cat README.md'
                echo 'Test finished....'
            }
        }   
        stage('Deploy') {
            steps {
                echo 'Deploying... FROM NEW BRANCH'
                sh 'ls -la'
                echo 'Deploy finished....'
            }
        }
    }  
    post {
        success {
            echo 'Pipeline succeeded!  HO-HO-HO !!! FROM -- OTHER -- BRANCH'
        }
        failure {
            echo 'Pipeline failed!   HO-HO-HO !!! FROM -- OTHER --  BRANCH '
        }
    }
}
