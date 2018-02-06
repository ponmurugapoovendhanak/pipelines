pipeline {
    agent any
    stages {
        stage('Clone'){
          
                git url: 'https://github.com/ponmurugapoovendhanak/pipelines.git'
            }
        

        stage('maven_deploy'){
             sh 'mvn deploy'
           
            }
        }
    }
