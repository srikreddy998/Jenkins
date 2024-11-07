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
                echo "New Line 2"
            }
        }
        stage('Test') {
            steps {
                echo "Testing.. 4321"
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
