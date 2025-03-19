pipeline {
	agent tomcat 	
	stages {
		stage('git Checkout') {
			steps {
				git branch: 'main', url: 'https://github.com/Ravichandu-git/java-example.git' 
			}
		}
		
		stage('Build') {
			steps {
				sh 'mvn clean install'
			}
		}
	}
}
