pipeline{
    agent any
    parameters{
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
        choice(name: 'Env', choices: ['Dev', 'preprod', 'prod'])
    }
    stages{
         stage('Deployy'){
            steps{
                echo "Deploying to ${params.Env} environment"
            }
        }
        stage('Build'){
            steps{
                echo 'Building the application'
            }
        }
        stage('Test'){
            steps{
                echo 'Testing the application'
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deploying the application'
            }
        }
    }
}