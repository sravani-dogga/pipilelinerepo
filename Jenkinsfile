pipeline {
agent any
stages{
stage('checkout'){
steps{
cleanWs()
echo 'checking out remote repo'
git changelog:false, credentialsId:'ec2-user', poll:false, url:'https://github.com/sravani-dogga/pipilelinerepo.git'
}
}
}
}
