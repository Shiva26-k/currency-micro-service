pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                echo "This stage from main branch"
            }
        }
        stage('scan'){
            steps{
                echo "This stage from main branch"
            }
        }
        stage('test'){
            steps{
                echo "deploy stage from main branch"
            }
        }
        stage('docker'){
            steps{
                echo "docker stage developed"
            }
        }
        stage('deploy'){
            steps{
                echo "deploying in prod"
            }
        }
    }
}   
