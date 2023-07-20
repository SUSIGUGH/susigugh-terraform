pipeline {
    agent any

    stages {
        stage('Integration - Connect to GitHub') {
            steps {
                sh 'ls -ltr'
                sh 'terraform init'
                sh 'terraform plan'
                sh 'terraform destroy -auto-approve'
                sh 'terraform apply -auto-approve'
                sh 'terraform destroy -auto-approve'
            }
        }
    }
}
