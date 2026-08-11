pipeline {
    agent any

    stages {

        stage('Compile') {
            steps {
                echo 'Compiling Java Program...'
                bat 'javac AddNumbers.java'
            }
        }

        stage('Run') {
            steps {
                echo 'Running Java Program...'
                bat 'java AddNumbers'
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