pipeline {
    agent any

    stages {
        stage('Build Stage') {
            steps {
                echo 'Compiling..'
                sh "mvn clean compile"
            }
        }
        stage('Test Stage') {
            steps {
                echo 'Testing..'
                sh "mvn test"
            }
        }
        stage('Package Stage') {
            steps {
                echo 'Packaging....'
                sh "mvn package"
                archiveArtifacts artifacts: '**/target/*.war', fingerprint: true
            }
        }
        stage('Run Stage') {
            steps {
                echo 'Running....'
                sh "/home/hitham/hitham/private_projects/deployments/shell_demo.sh"
            }
        }
    }
}