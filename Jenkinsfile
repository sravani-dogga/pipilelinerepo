pipeline {
    agent any 
    stages {
        stage('checkout') { 
            steps {
                echo "checking put repository"
git changelog:false, credentials: "scriptedpipeline", poll:false, url:"https://github.com/sravani-dogga/pipilelinerepo.git" 
            }
        }
        stage('Test') { 
            steps {
                echo "build stage"
            }
        }
        stage('Deploy') { 
            steps {
               echo "deploy stage"
            }
        }
    }
}
