pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    if (isUnix()) {
                        sh 'javac division.java'
                        sh 'java division'
                    } else {
                        bat 'javac division.java && java division'
                    }
                }
            }
        }
    }
}