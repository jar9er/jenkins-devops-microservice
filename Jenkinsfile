pipeline {
	agent { docker {image 'maven:3.6.3'}}
	stages {
		stage('Build'){
			steps {
				echo "Build"
				sh 'mvh --version'
			}
		}
		stage('Test'){
			steps {
				echo "Test"
			}
		}
		stage('Integration Test'){
			steps {
				echo "Integration Test"
			}
		}
	}
	post {
		always {
			echo "I am awesome. I run always"
		}
		success {
			echo "I am awesome. I run when you succeed"
		}
		failure {
			echo "I am awesome. I run when you fail"
		}
	}
}
