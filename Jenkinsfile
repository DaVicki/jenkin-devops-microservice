// SCRIPTED - stage blocks are optional
// node {
// 	echo "Build"
// 	echo "Test"
// 	echo "Test"
// }

// DECLARATIVE
pipeline {
	agent {
		docker {
			image 'maven:3.6.3'
		}
	}
	// agent any
	stages {
		stage('Build') {
			steps {
				sh 'mvn --version'
				echo "Build"
			}
		}
		stage('Test') {
			steps {
				echo "Test"
			}
		}
		stage('Integration Test') {
			steps {
				echo "Integration Test"
			}
		}
	} post {
		always {
			echo 'Im awesome. I run always'
		}
		success {
			echo 'I run when you are successful'
		}
		failure {
			echo 'I run when you fail'
		}
	}
}
