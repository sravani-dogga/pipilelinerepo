pipeline {
    agent any 
    stages {
        stage('checkout') { 
            steps {
                echo "checking put repository"
git changelog:false, credentilas: "scriptedpipeline", pull:false, url:"https://github.com/sravani-dogga/pipilelinerepo.git" 
            }
        }
        stage('Test') { 
            steps {
                // 
            }
        }
        stage('Deploy') { 
            steps {
                // 
            }
        }
    }
}
