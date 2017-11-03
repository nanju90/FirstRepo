pipeline {
    agent any
    tools { 
        maven 'maven_3_5_2' 
        jdk 'jdk1.8.0_131'
    }
    stages {
        stage ('Initialize') {
            steps {
                sh '''
                    echo "PATH =PATH"
                    echo "M2_HOME = PATH"
                ''' 
            }
        }

        stage ('Build') {
            steps {
                echo 'This is a minimal pipeline.'
            }
        }
    }
}
