pipeline {
    tools {
        jdk 'JAVA_HOME2'      
        maven 'M2_HOME2'   
    }
    agent {
    node {
    label 'winslave'
    }
    }

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
        stage('test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('package') {
            steps {
                sh 'mvn package'
    }
}

    }
}
