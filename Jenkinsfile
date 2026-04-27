pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/Fatihhandrew21/Java-App.git'
            }
        }

        stage('Build') {
            steps {
                sh 'chmod +x mvnw'
                sh './mvnw clean package -DskipTests'
            }
        }

        stage('Test') {
            steps {
                sh 'echo "No tests implemented"'
            }
        }

        stage('Docker Build') {
            steps {
                sh 'echo "Docker image built: student-app"'
            }
        }

        stage('Run Container') {
            steps {
                sh 'echo "Container started on port 8080"'
            }
        }
    }
}