pipeline {
    agent any
    environment{
        CC = 'clang'
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
		echo "NODE_NAME ${env.NODE_NAME}"
		echo "JAVA_HOME ${env.JAVA_HOME}"
		echo "WORKSPACE ${env.WORKSPACE}"
		echo "BUILD_URL ${env.BUILD_URL}"
		echo "BUILD_NUMBER ${env.BUILD_NUMBER}"
		echo "BUILD_TAG ${env.BUILD_TAG}"
		echo "JENKINS_URL ${env.JENKINS_URL}"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying....${env.CC}"
		sh 'printenv'
            }
        }
    }
}
