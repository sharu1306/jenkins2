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
                echo 'Testing is happening here...'
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
        emailext body: 'Summary', replyTo: 'sharat.g.13@gmail.com', subject: 'Jenkins Pipeline', to: 'sharat.g.13@gmail.com'
        }
    }
}
