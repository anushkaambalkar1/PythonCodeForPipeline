pipeline{
    agent any

    stages{
        stage('Git Clone'){
            steps{
                git branch: '', credentialsId: 'CICDJenkins', url: ''
            }
        }
    }

    post{
        success{
            echo 'Pipeline successfully completed!'
        }
        failure{
            echo 'Pipeline failed. Please check the logs for more info!'
        }
    }
}