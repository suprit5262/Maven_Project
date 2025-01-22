pipeline {
    agent none  

    stages {
        stage('Cloning') {
            agent { label 'linuxslave' }  

            tools {
                jdk 'JAVA_HOME2'  
                maven 'M2_HOME2'  
            }

            steps {
                git 'https://github.com/suprit5262/Maven_Project.git'
                sh 'mvn compile'
            }
        }
    }
}
