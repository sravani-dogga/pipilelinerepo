pipeline {
    agent any 
    stages {
        stage('checkout') { 
            steps {
                echo "checking put repository"
git changelog:false, credentialsId: "newuser", poll:false, url:"https://github.com/sravani-dogga/pipilelinerepo.git" 
            }
        }
        stage('Build') { 
            steps {
                echo "build stage is commited"
                sh 'mvn clean package'

            }
        }
        stage('Deploy') { 
            steps {
               echo "deploy stage"
               sh 'cp -rp $WORKSPACE /target/hello-world-maven /opt/tomcat9/webapps'
}
     }
    }
}
