// Powered by Infostretch 

timestamps {

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
}
