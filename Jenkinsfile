pipeline {
    tools {
        jdk 'JAVA_HOME'      
        maven 'M2_HOME'   
    }
    agent any

    stages {

        stage("git checkout") {
            steps {
                git 'https://github.com/suprit5262/Maven_Project.git'
              }
        }
        stage('compile') {
            steps {
                sh 'mvn compile'
                          
            }
        }             
        
    }
}
