pipeline {
    agent any

    stages {

        stage('Compile') {
            steps {
                echo 'Compiling Java Program...'
                bat 'javac SubNumbers.java'
            }
        }

        stage('Run') {
            steps {
                echo 'Running Java Program...'
                bat 'java SubNumbers'
            }
        }
    }

    post {
        success {
            echo 'Build Successful!'
        }

        failure {
            echo 'Build Failed!'
        }
    }
}