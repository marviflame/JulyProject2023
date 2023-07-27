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

        stage ("Ansible Version") {
            steps {
                sh 'ansible --version'
            }
        }

        stage ("Maven Version") {
            steps {
                sh 'mvn -v'
            }
        }

        stage ("Docker Version") {
            steps {
                sh 'docker version'
            }
        }

        stage ("Docker Version II") {
            steps {
                sh 'docker --version'
            }
        }

    }
}
