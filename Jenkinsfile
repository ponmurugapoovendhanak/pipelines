pipeline {
    agent any
    stages {
        stage('Clone'){
            steps{
                git url: 'https://github.com/ponmurugapoovendhanak/pipelines.git'
            }
        }
        

        stage('maven_deploy'){
            steps{
             sh 'mvn deploy'
                
            }
        }
        stage('maven_deploy_tomcat'){
            steps{
            sh 'cp /var/lib/jenkins/workspace/pipelines/target/pipeline.war /etc/tomcat7/Catalina/webapps/'
           
            }
        }
    }
}
