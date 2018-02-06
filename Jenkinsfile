pipeline {
    agent any
    stages {
        stage('Clone'){
            steps {
                git url: 'https://github.com/ponmurugapoovendhanak/pipelines.git'
            }
        }

        stage('maven deploy'){
        sh 'mvn deploy'
           
            }
        }
    }
