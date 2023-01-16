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

        stage('Build') {
            steps {
                bat 'mvn install'
            }
         }

    }
}