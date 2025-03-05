pipeline {
    agent any

    stages {
        // stage('clone') {
        //     steps {
        //       //  git branch: 'main', url: 'https://github.com/Damu9393/Terraform_CICD.git'
        //     }
        // }
        stage('init') {
            steps {
                sh 'terraform init'
            }
        }
         stage('plan') {
            steps {
                sh 'terraform plan'
            }
        }
    }
}
