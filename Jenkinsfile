pipeline {
    agent any 
    stages {
        stage('build') {
            steps {
                echo "Building some things!"
            }
        }
        stage('test') {
            steps {
                echo "Testing more things!"
            }
        }
        stage('push-to-prod') {
            input message: 'Are this version ready for Production?'
            submitter: 'DevOps'
            steps {
                echo "This has been approved for release to production!"
            }
        }
    }
}
