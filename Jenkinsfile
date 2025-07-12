pipeline{
    agent{
        label 'java-slave'
    }
    stages{
        stage('Build'){
            steps{
                echo "Build the application"
            }
        }
        stage('sonar'){
            steps{
                echo "scaning the application"
            }
        }
        stage('dockerIamge'){
            steps{
                echo "creating docker image"
            }
        }
        stage('deplotToDev'){
            steps{
                echo "Deplyoing in dev envrmnt"
            }
        }
        stage('deployToTest'){
            steps{
                echo "Deploying in test environment"
            }
        }
        stage('deployToStage'){
            when{
                branch 'release-*'
            }
            steps{
                echo "deploy to stage"
            }
        }
        stage('deplotToprod'){
            when{
                tag pattern : "v\\d{1,2}.\\d{1,2}.\\d{1,2}"
            }
            steps{
                echo "deploy to prodcution"
            }
        }
    }
}
