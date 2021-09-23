pipeline {
    agent any
    stages{
       stage('clone repo'){
       steps {
           echo 'clone repo'
           git branch: 'master',
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
        stage('Example') {
            input {
                 message "Can we deploy in production?"
                 ok "yes"
                 submitter "Pritam Ramteke"
                 parameters {
                       strings(name: "PERSON", defaultvalue: "Mr. Jenkins" , description: "want to contine")
                 }
            }
            steps {
                echo "Hello,{$PERSON} Nice to meet you"

             }
 
         }
      }
   }
  

