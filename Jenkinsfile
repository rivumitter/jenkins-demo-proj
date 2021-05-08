pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                echo 'Hello Build'
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
