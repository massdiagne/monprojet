pipeline {
	agent any
	tools {
		maven '3.6.3'
	}
	
	stages {
		stage('Source') {
			steps{
				git branch: 'master', url: 'https://github.com/massdiagne/monprojet.gitt'
		}
		
		stage('Build') {
			steps {
				bat 'mvn clean package'
			}
		}
	}
