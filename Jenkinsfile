pipeline {
    tools {
        jdk 'JAVA_HOME2'      
        maven 'M2_HOME2'   
    }
    agent {label 'winslave'}

    stages {

        stage("git checkout") {
            steps {
                git 'https://github.com/suprit5262/Maven_Project.git'
              }
        }
        stage('compile') {
            steps {
                bat 'mvn compile'
                          
            }
        }             
        stage('test') {
            steps {
                bat 'mvn test'
            }
        }
        stage('package') {
            steps {
                bat 'mvn package'
    }
}

    }
}
