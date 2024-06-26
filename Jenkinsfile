pipeline {
  agent any

  environment {
    AWS_DEFAULT_REGION = 'ap-south-1'
  }

  stages {
    stage('Checkout') {
      steps {
        git 'https://github.com/your-repo/your-terraform-repo.git'
      }
    }

    stage('Terraform Init') {
      steps {
        sh 'terraform init'
      }
    }

    stage('Terraform Plan') {
      steps {
        sh 'terraform plan -out=plan.tfplan'
      }
    }

    stage('Terraform Apply') {
      steps {
        sh 'terraform apply plan.tfplan'
      }
    }
  }
}

