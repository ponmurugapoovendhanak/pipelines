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
            sh 'scp -i ganga_key.pem workspace/pipelines/target/pipeline.war centos@34.208.231.143:/var/lib/tomcat/webapps/pipeline.war'
           
            }
        }
    }
}
