pipeline {
    agent any
    tools { 
         maven 'maven_3_5_2' 
         jdk 'jdk1.8.0_131' 
    }
    stages {
        
        stage ('Build') {
            steps {
                sh 'mvn -Dmaven.test.failure.ignore=true install' 
            }
            post {
                success {
                    junit 'target/surefire-reports/**/*.xml' 
                }
            }
        }
    }
}
