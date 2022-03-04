pipeline{
  agent any
    stages{
       stage('hosting application'){
        steps{
          sh "ls"
           sh "aws cloudformation create-stack --stack-name mystacknewfinal3 --template-body file://awscli/stack.yml --region us-east-1" 
           sh "aws ec2 create-key-pair --key-name MyKeyPair"
        }
       }
      }
    }
