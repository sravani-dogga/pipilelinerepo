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
stage('build'){
steps{
echo 'build'
sh """
ls -ltr
which mvn
mvn clean package
"""
}
}
stage('deploy stage'){
steps{
echo 'deplay stage'
sh """
echo $WORKSPACE
"""
}
}
}
}
