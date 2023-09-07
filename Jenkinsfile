pipeline {
    agent any

    stages {
        stage('git') {
            steps {
                git credentialsId: 'jenkins', url: 'git@github.com:sravandevops15/maven-simple.git'
            }
        }
        stage('maven'){
            steps{
                sh 'mvn clean package'
            }
        }
    }
}
