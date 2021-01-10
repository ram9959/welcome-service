pipeline {
	agent any
	
	stages {
		stage ('Build') {
			git url: 'https://github.com/ram9959/welcome-service'	
			steps{
				withMaven(maven: 'maven_3_6_3') {
					sh 'mvn clean compile'
				}
			}
			
		}
		
		
		stage ('Test') {
			git url: 'https://github.com/ram9959/welcome-service'
			steps{
				withMaven(maven: 'maven_3_6_3') {
					sh 'mvn clean compile'
				}
			}		
		}
		
		stage ('Deployment') {
			git url: 'https://github.com/ram9959/welcome-service'
			steps{
				withMaven(maven: 'maven_3_6_3') {
					sh 'mvn deploy'
				}
			}
		}
	
	
	}

}
