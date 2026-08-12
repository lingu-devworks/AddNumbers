pipeline {
    agent any

    stages {

        stage('Compile') {
            steps {
                echo 'Compiling Java Program...'
                bat 'javac MultipleNumbers.java'
            }
        }

        stage('Run') {
            steps {
                echo 'Running Java Program...'
                bat 'java MultipleNumbers'
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