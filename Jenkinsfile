pipeline {
    agent any

    
    stages {
        stage('Login and Push'){
            steps {
                script{
                    withDockerRegistry(credentialsId: 'Docker') {
                        docker.build('omerdl/flaskapp').push('latest')
                    }
                }
            }
        }
    }
}