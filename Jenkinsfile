pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                def version = '1.0'
                sh "echo Building version ${version}..."
                sh 'echo "Building..."'
                }
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Testing..."'
            }
        }
        stage('Deploy') {
            steps {
                script {
                def params=[
                    new StringParameterValue('para1', 'value1'),
                    new StringParameterValue('para2', 'value2'),
                ]
                def jobName='my-other-job'
                build job: jobName, parameters: params
                }
            }
        }
    }
}
