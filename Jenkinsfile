pipeline {
	agent any
	
	stages{
		stage{
			('Compile Stage') {
				steps{
					withMaven(maven : 'maven_actual'){
						sh 'mvn test'	
					}
				}
			}
		}
	}
}