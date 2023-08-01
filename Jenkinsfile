pipeline {

    agent any
    stages {

        stage ("Environment Variable") {
            steps {
                sh 'printenv'
            }
        }

        stage ("Git Version") {
            steps {
                sh 'git version'
            }
        }


        stage ("Maven Version") {
            steps {
                sh 'mvn -v'
            }
        }
        
        stage ("Java Version"){
            steps {
                sh 'java --version'
            }
        }

    }
}
