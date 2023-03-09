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
                def params = [
                    new StringParameterValue('para1', 'value1'),
                    new StringParameterValue('para2', 'value2'),
                ]
                def jobName = 'my-other-job'
                build job: jobName, parameters: params
            }
        }
    }
}
