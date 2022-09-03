// Powered by Infostretch 

timestamps {

node () {

	stage ('job123 - Checkout') {
 	 checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'ec2-user', url: 'https://github.com/sravani-dogga/pipilelinerepo.git']]]) 
	}
}
}