pipeline {
    agent any

    stages {
        stage('Compile and Run') {
            steps {
                script {
                    if (isUnix()) {
                        sh 'javac SubNumbers.java'
                        sh 'java SubNumbers'
                    } else {
                        bat 'javac SubNumbers.java && java SubNumbers'
                    }
                }
            }
        }
    }
}