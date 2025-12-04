pipeline {
    agent any

    tools {
        maven 'Maven-3' 
        jdk 'Java-17'   
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
                echo 'Code checked out from GitHub.'
            }
        }

        stage('Test') {
            steps {
                echo 'Running Maven tests...'
                bat 'mvn clean test' 
            }
        }
    }
}