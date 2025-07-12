pipeline{
    agent{
        label 'java-slave'
    }
    environment{
        DEPLOY_TO = 'production'
    }
    stages{
        stage('Build'){
            steps{
                echo "Running a build stage"
            }
        }
        stage('scan'){
            when{
                allOf{
                    branch 'production'
                    environment name : 'DEPLOY_TO' , value : 'production'
                }
            }
            steps{
                    echo "Build by using when consitions"
            }
        }
    }
}
