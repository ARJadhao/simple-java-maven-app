pipeline {
    agent {
        docker {
            image 'maven:3.8.1-adoptopenjdk-11' 
            args '-v /root/.m2:/root/.m2' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn package -Dmaven.test.skip=false' 
                script{
                    try{
                        def v = 7/0
                    }catch(e){
                        throw e                    
                    }
                }
            }
        }
    }
}
