pipeline {

    agent any

    stages {

        stage ("Environment Variable") {
            steps {
                script {
                   sh 'printenv'
                }   
            }
        }

        stage ("Git Version") {
            steps {
                script {
                   sh 'git version'
                }   
            }
        }


        stage ("Maven Version") {
            steps {
                script {
                   sh 'mvn -v'
                }   
            }
        }
        
        stage ("Javac Version"){
            steps {
                script {
                   sh 'java --version'
                }   
            }
        }

    }
}
