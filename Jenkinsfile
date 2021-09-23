pipeline {
    agent any
    stages {
        stage('Example Build') {
            steps {
                echo 'Hello, Maven'
                sh 'mvn --version'
                sh 'mvn install'
            }
        }
        stage('Example Test') {

            steps {
                echo 'Hello, JDK'
                sh 'java -version'
            }
        }
    }
}
