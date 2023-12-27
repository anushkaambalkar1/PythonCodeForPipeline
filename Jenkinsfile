pipeline{
    agent any

    stages{
        stage('Git Clone'){
            steps{
                git branch: 'main', credentialsId: 'CICDJenkins', url: 'https://github.com/anushkaambalkar1/PythonCodeForPipeline.git'
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
