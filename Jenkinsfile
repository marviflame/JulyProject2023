pipeline {

    agent any

    stages {

        stage ("Cleanup Workspace") {
            steps {
                cleanWs()
            }   
        }

        stage ("Checkout From SCM") {
            steps {
                git branch: 'main', credentialsId: 'marviflame', url: 'https://github.com/marviflame/JulyProject2023.git'
            }   
        }

        stage ("Build Application") {
            steps {
                sh 'maven clean package'
            }   
        }
        
       stage ("Test Application") {
            steps {
                sh 'mvn test'
            }   
        }

        stage ("Sonarqube Analysis") {
            steps {
                script {
                     withSonarQubeEnv(credentialsId: 'sonar-token') {
                      sh 'mvn sonar:sonar'  
                    }
                }    
            }
        }    

    }
}
