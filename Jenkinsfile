pipeline {
    agent any
    options {
        quietPeriod(3000)  // 3000 seconds delay before starting the pipeline
    }
    triggers {
        pollSCM('H/5 * * * *')  // Polls for SCM changes every 5 minutes
    }
    stages {
        stage('Initialize') {
            steps {
                echo 'Initializing...'
            }
        }
        stage('Build') {
            steps {
                echo 'Building project...'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
    }
}
