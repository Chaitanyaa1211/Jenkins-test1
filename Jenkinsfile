pipeline {
    agent any
    
    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t jenkins-demo:v1 . '
                
            }
        }
        stage('Run Container') {
            steps {
                sh 'docker run jenkins-demo:v1'
            }
        }
    }
}
