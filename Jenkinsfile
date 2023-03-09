pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Building..."'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Testing..."'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploying..."'
                def params = [
                    new StringParameterValue('para1', 'abc'),
                    new StringParameterValue('para2', 'xyz'),
                    new StringParameterValue('para3', 'value3')
                ]
                def jobName = 'my-other-job'
                build job: jobName, parameters: params
            }
        }
    }
}
