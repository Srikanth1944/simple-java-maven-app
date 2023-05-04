pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'build application'
            }
        }
      
      stage('Test') {
            steps {
                echo 'Test application'
            }
        }
        stage('Deploy') {
            steps {
                echo 'deploy application'
            }
        }
    }
    post{
        always{
            emailext body: 'Summery', subject: 'Jenkins pipeline', to: 'srinimmala916@gmail.com'
        }
    }
}
