pipeline {
    agent { 
        node {
            label 'docker-agent-python'
            }
      }
  triggers {
    pollSCM '* * * * *'
  }
    stages {
        stage('Build') {
            steps {
                echo "Building.."
                sh '''
                echo "doing build stuff.."
                '''
                echo "Building..2.0"
                sh '''
                echo "doing build stuff.."
                '''
                
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                sh '''
                echo "doing test stuff.."
                '''
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver....'
                sh '''
                echo "doing delivery stuff.."
                '''
            }
        }
    }
}
