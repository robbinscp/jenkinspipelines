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
            input {
                message 'Is this version ready for Production?  Yes, No, Maybe?'
                ok 'Yes'
                submitter 'Roadies-Admins, DevOps'
            }
            steps {
                echo "This has been approved for release to production"
                echo "Pushing code to prod!"
            }
        }
    }
}
