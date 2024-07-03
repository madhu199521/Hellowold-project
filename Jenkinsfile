pipeline {
    agent {label 'slave'}

    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        jdk 'Java'
        maven "Maven"
    }

    stages {
        stage('Git Clone') {
            steps {
                git branch: 'main',
                url: 'https://github.com/madhu199521/Hellowold-project.git'
            }
        }    
        stage('Maven Build') {
            steps {
                sh 'mvn clean package'
            }
        }        
               
            }
}
