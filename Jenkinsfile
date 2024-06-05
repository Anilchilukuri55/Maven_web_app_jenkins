pipeline{
    agent any
    environment {
        PATH = "$PATH:/opt/apache-maven-3.9.7/bin"
    }
    stages{
       stage('GetCode'){
            steps{
				git branch: 'main',
                url: 'https://github.com/Anilchilukuri55/Maven_web_app_jenkins.git'
            }
         }        
       stage('Build'){
            steps{
                sh 'mvn clean package'
            }
         }       
    }
}
