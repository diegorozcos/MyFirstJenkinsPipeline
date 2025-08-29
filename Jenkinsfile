pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/diegorozcos/MyFirstJenkinsPipeline'
            }
        }
        stage('Ejecutar script') {
            steps {
                sh 'chmod +x myscript'
                sh './myscript'
            }
        }
        stage('Ejecutar script de Python') {
            steps {
                sh 'python3 sum.py'
            }
        }
    }
}

