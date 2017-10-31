pipeline{
	agent any
	
	stages{
	
	
	
		stage('Compile stage') {
			steps{
				withMaven(maven : 'MAVEN_TOOL') {
				   sh 'mvn clean compile'
				}
			}
		}
		
		stage('Testing stage') {
			steps{
				withMaven(maven : 'MAVEN_TOOL') {
				   sh 'mvn test'
				}
			}
		}
		
		
	
	}
	
}
