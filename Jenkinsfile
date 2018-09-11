pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh "mvn clean package"
               sudo sh "docker build . -t tomcatwebapp:${env.BUILD_ID}"

            }
            
        }
    }
    
}