pipeline {
    agent any

    stages {
        stage('build') {
            steps {
		git 'https://github.com/rivumitter/jenkins-demo-proj.git'
                echo 'Hello Build'
            }
        }
	stage('test') {
            steps {
                echo 'Hello Test'
            }
        }
    }
	
}
