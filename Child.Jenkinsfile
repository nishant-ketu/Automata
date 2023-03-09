pipeline {
    agent any
    stages {
        stage('Build Child') {
            steps {
                sh 'echo "Building Child.."'
            }
        }
        stage('Test Child') {
            steps {
                sh 'echo "Testing Child..."'
            }
        }
        stage('Deploy Child') {
            steps {
                sh 'echo "Deploying Child..."'
            }
        }
    }
}
