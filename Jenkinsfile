pipeline {
    agent any
	parameters {
		string(name: 'VERSION', defaultValue: '79', description: '')
	}
    stages {
        stage('build') {
            steps {
                echo 'Hello Build, Pulling brachName=' + env.BRANCH_NAME
            }
        }
	    stage('test') {
            when {
                expression {
                   params.VERSION == '79'
                }
            }
            steps {
                echo 'Hello Test'
            }
        }
    }
	
}
