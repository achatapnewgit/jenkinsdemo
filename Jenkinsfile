pipeline {
    agent { docker { image 'maven:3.9.6-eclipse-temurin-17-alpine' } }
    environment{
        name = "anurag"
        username = credentials('username')
    }
    stages {
        stage('build') {
            steps {
                echo "executing build stage"
                
                sh 'mvn --version'
                echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL} and name is ${env.name} and I am ${env.title} "
            
                withCredentials([usernamePassword(credentialsId: 'cred', passwordVariable: 'password', usernameVariable: 'username')]) {
                        
                    }
            }
        }
    }
}
