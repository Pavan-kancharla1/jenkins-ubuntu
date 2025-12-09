pipeline {
	agent {
		docker {
			image 'ubuntu:26.04'
			args '-u 0:0'   // run container as root
			}
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
				sh 'ps -ef| grep amazon'
			}
		}
		stage('Install python') {
			steps {
			sh '''
				apt-get update
				apt-get install -y python3
			'''
				}
		}
		stage('Run Python Script') {
			steps {
				sh 'python3 src/hello.py'
			}
		}
	}
}

