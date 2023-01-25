pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building progress is going on stop..'
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
       emailext body: 'hello', subject: 'wish', to: 'sharat.g.13@gmail.com'
        }
    }
}
