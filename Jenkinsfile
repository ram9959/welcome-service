pipeline {
	agent any
	
	stages {
		stage ('Build') {
			steps{
				withMaven(maven: 'maven_3_6_3') {
					sh 'mvn clean install'
				}
			}
			
		}
		
		
		stage ('Test') {
			steps{
				withMaven(maven: 'maven_3_6_3') {
					sh 'mvn clean compile'
				}
			}		
		}
		
		stage ('Deployment') {
			steps{
				withMaven(maven: 'maven_3_6_3') {
					sh 'mvn deploy'
				}
			}
		}
	
	
	}

}
