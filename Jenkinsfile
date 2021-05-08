pipeline {
    agent any
	parameters {
		string(name: 'VERSION', defaultValue: '79', description: '')
		booleanParam(name:'EXECUTE_TESTS', defaultValue: true, description: '')
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
                   params.EXECUTE_TESTS == true
                }
            }
            steps {
                echo 'Hello Test'
            }
        }
    }
	
}
