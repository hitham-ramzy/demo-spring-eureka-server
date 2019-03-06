pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Compiling..'
                sh "mvn clean compile"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh "mvn test"
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                sh "mvn deploy"
            }
        }
    }
}