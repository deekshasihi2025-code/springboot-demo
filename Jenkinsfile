pipeline {
    agent {
        label 'slave'
    }

    stages {
        stage('Test Slave') {
            steps {
                sh 'hostname'
                sh 'java -version'
                sh 'mvn -version'
                sh 'docker --version'
            }
        }

        stage('Build') {
            steps {
                sh 'java -version'
                sh 'mvn -version'
                sh 'mvn clean package -DskipTests'
            }
        }
    }
}
