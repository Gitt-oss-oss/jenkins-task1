pipeline {
    agent any
    
    environment {
        APP_PORT = '9090'
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn -B clean package -DskipTests'
            }
        }
        stage('Unit Test') {
            steps {
                 sh 'mvn -B test'
            }
        }
    }
}
