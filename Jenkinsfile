pipeline{
    agent {
        label 'java-slave'
    }
    environment{
        TODAY_DAY = 'saturday'
    }
    stages{
        stage('Build'){
            // when{
            //     environment name : 'TODAY_DAY' , value : 'saturday'
            // }
            when{
                expression{
                    BRANCH_NAME ==~ /(prod|hotfix)/
                }
            }


            steps{
                echo "this stage will be execute for when example "
            }
        }
    }
}
