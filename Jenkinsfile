pipeline {
	agent any
	
	stages {
		stage ('Build') {
			steps{
				withMaven(maven: 'maven_3_6_3') {
					bat './mvnw clean install -DskipTests'
				}
			}
			
		}
	}

}
