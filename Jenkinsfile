pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing is happening...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying is happening.....'
            }
         
        }
       
    }
    post{
        always{
        emailext body: 'Summary', replyTo: 'k.g.sharataa124@gmail.com', subject: 'Jenkins Pipeline', to: 'k.g.sharataa124@gmail.com'
        }
    }
}
