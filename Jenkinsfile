
pipeline {
    agent any

    tools{
    Maven:'M3'
    }
    
    stages {
        stage('Build') {
           
            steps {
                echo 'building..'
                sh 'mvn clean install'
            }
        
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
