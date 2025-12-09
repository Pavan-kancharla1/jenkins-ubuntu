pipeline {
	agent {
		docker {image 'ubuntu:26.04'}
	}
	stages {
		stage('checkout') {
			steps{
				git branch: 'main',
				url: 'https://github.com/Pavan-kancharla1/jenkins-ubuntu.git'
				}
		}
		stage('Test') {
			steps {
				sh 'ls'
				sh 'pwd'
			}
		}
	}
}

