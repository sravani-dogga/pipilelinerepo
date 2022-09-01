pipeline {
    agent any 
    stages {
        stage('checkout') { 
            steps {
                echo "checking put repository"
git changelog:false, credentialsId: "newuser", poll:false, url:"https://github.com/sravani-dogga/pipilelinerepo.git" 
            }
        }
        stage('Test') { 
            steps {
                echo "build stage"
sh***
ls -ltr
mvn clean package
***
            }
        }
        stage('Deploy') { 
            steps {
               echo "deploy stage"
sh***
echo $WORKSPACE
***
            }
        }
    }
}
