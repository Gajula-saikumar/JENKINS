pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build app'
            }
        }
        stage('test') {
            steps {
                echo 'test app'
            }
        }
        stage('deploy') {
            steps {
                echo 'deploy app'
            }
        }
       
    }
    post{
        always{
            emailext body: 'summary', subject: 'Pipeline status', to: '221710405014@gitam.in'
        }
    }
}
