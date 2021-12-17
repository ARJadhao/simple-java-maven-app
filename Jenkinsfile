pipeline {
    agent any
    tools { 
        maven 'maven' 
        jdk 'JAVA_HOME' 
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
