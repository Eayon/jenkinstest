
pipeline {
    agent any

    tools{
    maven 'Maven 3.5.0'
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
