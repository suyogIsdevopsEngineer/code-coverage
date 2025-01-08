pipeline{
    agent any
    tools {
        maven 'Maven'
    }
    stages{
        stage('git checkout'){
            steps{
                git branch: 'main', credentialsId: 'aec361ff-c7d8-4a22-bf63-9c74423ce78c', url: 'https://github.com/suyogIsdevopsEngineer/code-coverage.git'
            }
        }
        stage('build'){
            steps{
                sh 'mvn clean install'
            }
        }
    }
}