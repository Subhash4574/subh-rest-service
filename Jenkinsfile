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

         stage('run') {
             steps {
                 bat 'java -jar target/subh-rest-service-0.0.1-SNAPSHOT.jar'
             }
         }

    }
}