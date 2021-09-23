pipeline {
    agent any
    stages{
       stage('clone repo'){
       steps {
           echo 'clone repo'
           git branch: 'master'
           url: 'https://github.com/prit2477/solid-octo-guacamole.git'
}
}

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
