pipeline{
  agent any
    stages{
       stage('hosting application'){
        steps{
          sh "ls"
           sh "aws cloudformation create-stack --stack-name mystacknewfinal93 --template-body file://shiva_code.yml --region us-east-2" 
           sh "aws ec2 create-key-pair --key-name MyKeyPair"
        }
       }
      }
    }
