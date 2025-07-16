pipeline {
    agent any

    stages {
        // stage('Clean Workspace') { // (Optional) Cleans old files before cloning
        //     steps {
        //         cleanWs()
        //     }
        // }
        // stage('Clone Repository') {
        //     steps {
        //         git branch: 'main', url: 'https://github.com/Damu9393/Terraform_CICD.git'
        //     }
        // }
        stage('Terraform Init') {
            steps {
                sh 'terraform init'
            }
        }
        stage('Terraform Plan') {
            steps {
                sh 'terraform plan'
            }
        }
        stage('Terraform Apply') {
            steps {
                sh 'terraform apply -auto-approve'
            }
        }
    }
}
