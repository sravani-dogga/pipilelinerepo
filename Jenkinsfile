// Powered by Infostretch 

//timestamps {

node () {

	stage ('srcriptedjob - Checkout') {
 	 checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'ec2-user12', url: 'https://github.com/sravani-dogga/pipilelinerepo.git']]]) 
	}
	stage ('srcriptedjob - Build') {
 			// Shell build step
sh """ 
echo $WORKSPACE
mvn clean package 
 """ 
	}
}
}//

pipeline {
    agent any 
    stages {
        stage('checkout') { 
            steps {
                echo "checking remote repo"
git changelog:false, credentials:"scriptedpipeline",pull:false,url:"https://github.com/sravani-dogga/pipilelinerepo.git"
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
