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
                echo "build stage"
sh ***
ls -ltr
which mvn
mvn clean package
***

            }
        }
        stage('Deploy') { 
            steps {
               echo "deploy stage"
}
     }
    }
}
