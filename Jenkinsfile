pipeline {
    agent {
	node {
		label 'roboshop'
	     }
	  }
      environment {
        course = "devops"
      }
      options {
        disableConcurrentBuilds()
        timeout(time: 6, unit: 'SECONDS')
      }
    stages {
        stage('Build') {
            steps {
               script {
		         sh """
                     echo "building..." 
                     echo $course
                     sleep 5
                  """
   		}
            }
        }
        stage('Test') {
            steps {
                script {
		          sh """
                     echo "testing..." 
                  """
   		}
            }
        }
        stage('Deploy') {
            steps {
                script {
		          sh """
                     echo "deploying..." 
                  """
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
}
