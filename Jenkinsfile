pipeline {
    agent any

    stages {
        stage('Compile and Run') {
            steps {
                script {
                    if (isUnix()) {
                        sh 'javac Multiple.java'
                        sh 'java Multiple'
                    } else {
                        bat 'javac Multiple.java && java Multiple'
                    }
                }
            }
        }
    }
}