pipeline {
    agent { docker { image 'maven:3.9.6-eclipse-temurin-17-alpine' } }
    environment{
        name = "anurag"
    }
    stages {
        stage('build') {
            steps {
                echo "executing build stage"
                echo "hello Anurag"
                sh 'mvn --version'
                echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL} and name is ${env.name} and I am ${env.title} "
            
                
            }
        }
        stage('email'){
            steps{
                mail bcc: '', body: 'test', cc: '', from: '', replyTo: '', subject: 'test', to: 'achatapnew@gmail.com'
            }
        }
    }
}
