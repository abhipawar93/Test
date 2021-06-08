pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the application'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing the application'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application'
            }
        }
    }

    post
    {
        failure
        {
            emailext body: 'heyy pipeline is failed', subject: 'Pipeline failed', to: 'pawar.abhijeet996@gmail.com'
        }
    }
}
