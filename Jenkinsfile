pipeline {

    agent any

    stages {

        stage ('Build') {
            steps {
                withMaven(maven: 'maven_3_5_0') {
                    sh 'mvn test'
                }
            }
        }

        stage ('Deploy') {
            steps {
				{
                    sh 'mvn compile'
                    sh 'mvn install'
                }
            }

        }

    }

}