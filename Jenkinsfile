pipeline {
    agent any

    stages {
        stage('Deploy to Kubernetes') {
            steps {
                sh 'echo Deploying project...'
                sh 'kubectl apply -f deployment.yaml || true'
                sh 'kubectl apply -f service.yaml || true'
            }
        }
    }
}
