pipeline {
    agent none 
    stages {
        stage('Example Build') {
          #  agent { docker 'maven:3.8.1-adoptopenjdk-11' } 
             agent any
            steps {
                echo 'Hello, Maven'
                sh 'mvn --version'
            }
        }
            }
    }
