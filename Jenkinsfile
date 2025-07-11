pipeline{
    agent any
    environment {
        name = 'Shiva'
        course = 'cloud engineer'
    }
    stages{
        stage('Build'){
            steps{
                echo "welcome to hyderbad ${name}"
                echo "you are a ${course} right"
            }
        }
        stage('Test'){
            environment{
                name = 'Mahesh'
                city = 'kurnool'
            }
            steps{
                echo "Hello ${name}"
                echo "are you from ${city}"
            }
        }
    }
}
