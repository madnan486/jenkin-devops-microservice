/*node {
	stage('Build') {
		echo "Build"
	}
	stage('Test') {
		echo "Test"
	}
	stage('Integration Test') {
		echo "Integration Test"
	}
}*/

pipeline {
	agent any
	//agent { docker { image 'maven'} }
	
	stages{
		stage('Build'){
			steps {
				//sh 'mvn --version'
				echo "Build"
			}
		}
		stage('Test'){
			steps{
				echo "Test"
			}
		}
		stage ('Integration Test'){
			steps {
				echo "Integration Test"
			}
		}
	} 
	
	post {
		always {
			echo "I run always"
		}
		success {
			echo "I run when u sucessful"
		}
		failure{
			echo "I run when u fail"
		}
	}
}
