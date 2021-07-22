pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                echo 'build done'
            }
        }
        stage('Test') {
            steps {
                echo 'Test done'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy done'
            }
        }
        
    }
    post{
        always
        {
            emailext body: 'hi', subject: 'Pipeline status', to: 'devendrakadam.0403@gmail.com'
        }
    }
}
