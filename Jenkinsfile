pipeline {
	agent {
		docker {image 'ubuntu:26.04'}
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

