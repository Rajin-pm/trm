pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/Rajin-pm/trm.git',
                    credentialsId: 'github-pat'
            }
        }

        stage('Terraform Init') {
            steps {
                // Your Terraform Init steps here
            }
        }

        stage('Terraform Plan') {
            steps {
                // Your Terraform Plan steps here
            }
        }

        stage('Terraform Apply') {
            steps {
                // Your Terraform Apply steps here
            }
        }
    }
}

