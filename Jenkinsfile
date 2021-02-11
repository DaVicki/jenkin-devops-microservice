// SCRIPTED - stage blocks are optional
// node {
// 	echo "Build"
// 	echo "Test"
// 	echo "Test"
// }

// DECLARATIVE
pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
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
	}
}
