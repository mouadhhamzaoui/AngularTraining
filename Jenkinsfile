pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/mouadhhamzaoui/AngularTraining.git',
                    branch: 'main',
                    credentialsId: 'token'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
