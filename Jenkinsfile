pipeline {
    agent any

    stages {
        stage('Integration - Connect to GitHub') {
            steps {
                sh 'terraform init'
                sh 'terraform plan'
                sh 'terraform apply -auto-approve'
                sh 'terraform destory -auto-approve'
            }
        }
    }
}
