pipeline {
	agent {
		docker {image 'ubuntu:26.04'}
	}
	stage('checkout') {
                        steps{
                                git branch: 'main',
                                url: 'https://github.com/Pavan-kancharla1/jenkins-ubuntu.git'
                        }
        }
	stages {
		stage('Test') {
			steps {
				sh 'ls'
				sh 'pwd'
				sh 'ps -ef| grep amazon'
			}
		}
	}
}

