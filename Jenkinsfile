pipeline{
    agent any
    parameters{
        string(name: 'BRANCH', defaultValue: 'main')
        string(name: 'VERSION', defaultValue: '1.0')
    }
    environment{
        APP_Name ="MyApp"
    }
    stages{
        stage('checkout'){
            steps{
                echo "Checking out ${parameters.BRANCH}"
            }
        }
        stage('build'){
            steps{
                echo "building application"
            }
        }
        stage('unit testing'){
            steps{
                echo "testing a application"
            }
        }
        stage('code quality check'){
            steps{
                echo "checking code quality"
            }
        }
        stage('artifact name'){
            steps{
                echo "Packageing version ${parameters.VERSION}"
            }
        }
    }
}
