pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
		set AWS_ACCESS_KEY_ID=%AWS_ACCESS_KEY_ID%
		set AWS_SECRET_ACCESS_KEY=%AWS_SECRET_ACCESS_KEY%
		sh 'aws ec2 describe-instances'
            }
        }
    }
}
