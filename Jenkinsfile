pipeline {
    agent any
    environment{
        VERSION = "${env.BUILD_ID}"
    }
    stages {
        stage('Git checkout') {
            steps {
                git 'https://github.com/Ridlaw/Web-Application.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }       
    }
}
