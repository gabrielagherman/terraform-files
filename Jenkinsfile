pipeline{
  agent any
  environment {
  PATH = "{$path}:${getTerraformPath()}"
}

stages{
  stage('terraform init'){
    steps{
      sh 'terraform init'
      sh 'terraform plan'
      sh 'terraform apply -auto-approve'
    }
  }
