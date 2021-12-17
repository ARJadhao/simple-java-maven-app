pipeline {
    agent any
    tools { 
        maven 'Maven 3.6.0' 
        jdk 'jdk11' 
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
