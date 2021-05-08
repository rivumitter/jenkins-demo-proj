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
                    BRANCH_NAME == 'main'
                }
            }
            steps {
                echo 'Hello Test'
            }
        }
    }
	
}
