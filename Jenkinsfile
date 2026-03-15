pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/YOUR_USERNAME/devops-demo.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t devops-demo .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run -d -p 5000:5000 devops-demo'
            }
        }

    }
}
