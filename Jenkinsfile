pipeline {
    agent {
       label 'test-openhpi-rhel75.telco'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
		sh 'make'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh './helloworld'
            }
        }
    }
}
