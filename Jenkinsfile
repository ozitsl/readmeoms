pipeline {
    agent any

    
    stages {
        stage('Login and Push'){
            steps {
                script{
                    withDockerRegistry(credentialsId: 'Docker') {
                        docker.build('bjgomes/flaskapp').push('latest')
                    }
                }
            }
        }
    }
}