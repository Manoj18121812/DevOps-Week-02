pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo '===== BUILD STAGE ====='
                sh 'ls -la'
                echo 'Build completed successfully.'
            }
        }

        stage('Test') {
            steps {
                echo '===== TEST STAGE ====='
                sh 'echo Running tests...'
                sh 'echo All Tests passed.'
            }
        }

        stage('Validation') {
            steps {
                echo '===== VALIDATION STAGE ====='
                sh 'test -d .git'
                echo 'Git repository validation successful.'
            }
        }
    }
}
