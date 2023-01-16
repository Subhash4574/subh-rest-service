pipeline {
    agent any
    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                bat 'mvn clean compile'
            }
        }

        stage('install') {
            steps {
                bat 'mvn install'
            }
         }

    }
}