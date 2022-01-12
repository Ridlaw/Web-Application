pipeline {
    agent any
    environment{
        VERSION = "${env.BUILD_ID}"
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }       
    }
}}
