pipeline{
	agent any
	
	stages{
	
	
	
		stage('Compile stage') {
			steps{
				maven(maven:'maven_3_5_2') {
				   sh 'mvn clean compile'
				}
			}
		}
		
		stage('Testing stage') {
			steps{
				maven(maven:'maven_3_5_2') {
				   sh 'mvn test'
				}
			}
		}
		
		
	
	}
	
}
