pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                bat 'javac HelloWorld'
            }
        }

        stage('Test') {
            steps {
                bat 'HelloWorld'
            }
        }

        stage('Archive') {
            steps {
                archiveArtifacts artifacts: '*.class', fingerprint: true
            }
        }
    }
}
