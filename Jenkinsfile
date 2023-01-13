pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                sh 'make check'
            }
        }
    }
    post {
        always {
            junit '**/target/*.xml'
        }
        failure {
  emailext body: 'hi', subject: 'wish', to: 'thisiswasimnc@gmail.com'
        }
    }
}
