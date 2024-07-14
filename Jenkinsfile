//SCRIPT


//DECLARATIVE
pipeline {
	// agent any
	// agent {docker { image 'maven:3.6.3'}}
	agent {docker {image 'node:13.8'}}
	stages {
		stage ('Build'){
			steps {
				sh "node --version"
				echo "Build"
			}
		}
		stage ('Test'){
			steps {
				echo "Test"
			}
		}
		stage ('Integration'){
			steps {
				echo "Integration Test"
			}
		}

	} 
	
	post {
		always {
			echo 'Im awesome. I run always'
		}
		success{
			echo 'I run when you are successful'
		}
		failure {
			echo 'i run when you fail'
		}
	}

}
