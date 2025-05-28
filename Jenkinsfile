pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git branch: 'main', url:
        'https://github.com/Ram-9040/devops-ci-cd-demo.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t devops-demo .'
            }
        }

        stage('Run Docker Container') {
            steps {
                // Stop and remove any existing container (optional, safe to add)
                sh '''
                docker rm -f devops-demo-container || true
                docker run -d -p 80:80 --name devops-demo-container devops-demo
                '''
            }
        }
    }
}
