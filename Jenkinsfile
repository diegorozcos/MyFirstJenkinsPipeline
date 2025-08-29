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
                sh 'chmod +x myscript.sh'
                sh './myscript'
            }
        }
    }
}

