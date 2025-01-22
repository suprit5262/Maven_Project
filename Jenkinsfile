pipeline{
agent none
stages{
stage('cloning'){

tools{
jdk 'JAVA_HOME2'
maven 'M2_HOME2'
}
agent {
label 'linuxslave'
}
steps{
git 'https://github.com/suprit5262/Maven_Project.git'
sh 'mvn compile'


}
}
}
