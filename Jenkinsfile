pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                echo 'Hello Build, Pulling brachName=' + env.BRANCH_NAME
            }
        }
	    stage('test') {
            when {
                expression {
                    env.BRANCH_NAME == 'dev'
                }
            }
            steps {
                echo 'Hello Test'
            }
        }
    }
	
}
