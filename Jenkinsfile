pipeline {
    agent any 

    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo "Building.."
                echo "New Line"
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                sh '''
                python3 --version
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
