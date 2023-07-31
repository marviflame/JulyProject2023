pipeline {

    agent any
    stages {

        stage ("Environments Variable") {
            steps {
                sh 'printenv'
            }
        }

        stage ("Gits Version") {
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
