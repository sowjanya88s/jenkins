pipeline {
    agent {
        node {
            label 'roboshop'
        }
    }
       environment {
        course = "devops"
       }
    stages {
        stage('build') {
            steps {
                echo "building..."
                # exit 1
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
}
