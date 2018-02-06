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
    }
}
