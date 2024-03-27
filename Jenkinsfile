pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                // sh 'mvn --version'
                // sh 'node --version'
                echo 'Build'
                // Whats the path
                echo '$PATH'
                // What's the build number
                echo 'Build Number: $env.BUILD_NUMBER'
                // Whats the build id
                echo 'Build ID: $env.BUILD_ID'
                // What's the build tag
                echo 'Build Tag: $env.BUILD_TAG'
                // What's the build url
                echo 'Build URL: $env.BUILD_URL'
                // What's the job name
                echo 'Job Name: $env.JOB_NAME'
            }
        }
        stage('Test') {
            steps {
                echo 'Test'
            }
        }
        stage('Integration Test') {
            steps {
                echo 'Integration Test'
            }
        }
    } 
    post {
        always {
            echo 'I always run'
        }
        success {
            echo 'I run when successful'
        }
        failure {
            echo 'I run when failed'
        }
    }
}
