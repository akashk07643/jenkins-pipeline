pipeline {
    agent any

    parameters {
        string(name: 'BRANCH', defaultValue: 'main')
        string(name: 'VERSION', defaultValue: '1.0')
    }

    stages {

        stage('checkout') {
            steps {
                echo "Checking out ${params.BRANCH}"
            }
        }

        stage('build') {
            steps {
                echo "Building application"
            }
        }

        stage('test') {
            steps {
                echo "Testing application"
            }
        }

        stage('package') {
            steps {
                echo "Packaging version ${params.VERSION}"
            }
        }
    }
}
