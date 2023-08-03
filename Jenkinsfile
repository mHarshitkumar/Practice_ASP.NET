pipeline {
    agent any

    stages {
        stage('Success') {
            steps {
                echo 'Success Application'
            }
        }
        stage('Test') {
            steps {
                echo 'Test Application'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy Application'
            }
        }
    }
	
	post
	{
		always
		{
			emailext body: 'Summary', subject: 'Pipeline status', to: 'harshit.kumar@gingerwebs.co.in'
		}
	}
}
