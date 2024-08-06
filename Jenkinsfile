pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Your build steps here
            }
        }
        stage('Trigger Downstream Job') {
            steps {
                script {
                    build job: 'downstream-job-name', wait: false
                }
            }
        }
    }
}
