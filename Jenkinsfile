
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..',
                withMaven(Maven:'M3')(
                    // Maven installation declared in the Jenkins "Global Tool Configuration"
                    // Maven settings.xml file defined with the Jenkins Config File Provider Plugin
                    // Maven settings and global settings can also be defined in Jenkins Global Tools Configuration
      
                  // Run the maven build
                  sh "mvn clean compile"

                }
                    
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
