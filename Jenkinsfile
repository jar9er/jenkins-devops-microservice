pipeline {
	agent any
	stages {
		stage('Build'){
			steps {
				echo "Build"
				echo "$PATH"
				echo "BUILD_NUMBER: $env.BUILD_NUMBER"
				echo "BUILD_ID: $env.BUILD_ID"
				echo "JOB_NAME: $env.JOB_NAME"
				echo "BUILD_TAG: $env.BUILD_TAG"
				echo "BUILD_URL: $env.BUILD_URL"
				//sh 'mvn --version'
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
