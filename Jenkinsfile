pipeline {
    agent any

    tools {
        maven 'maven3'
    }

    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/allcodez/Calculator-Maven.git', branch: 'main'
            }
        }

        stage('Compile') {
            steps {
                sh 'mvn compile'
            }
        }

        stage('Unit Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}
