pipeline{
    agent{
        label 'java-slave'
    }
    environment{
        MONTH = 'july'
    }
    stages{
        stage('Dev_stage'){
            steps{
                echo "Deploy to dev environment"
            }
        }
        stage('Deploy_prod'){
            when{
                anyOf{
                    branch 'hotfix'
                    environment name :'MONTH' , value:'july'
                }
            }
            steps{
                echo "Deploy to prod"
            }
        }
    }
}
