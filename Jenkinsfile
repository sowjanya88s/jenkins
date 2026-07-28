pipeline {
    agent {
        node {
            label 'roboshop'
        }
    }
    stages {
        stage('build') {
            steps {
                echo "building..."
            }
        }
        stage('test') {
            steps {
                echo "testing..."
            }
        }
        stage('deploy') {
            steps {
                echo "deploying..."
            }
        }
    }
}
post {
	always {
	  echo 'i will say hello again!'
		}
	success {
	  echo 'pipeline success'
		}
	failure {
	  echo 'pipeline failure'
		}
	}
