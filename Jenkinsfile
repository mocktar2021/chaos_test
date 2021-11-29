pipeline {
    agent any
    stages {
	stage('Setup Variables') {
            steps {
                script {
                    configProperties = readProperties file: './config.properties'
                    Scenario = configProperties['Scenario']             
                }
            }
        } 
        stage('Data Injection Chaos automation') {
            steps {
		    script {
                sh echo "$Scenario"
		    }
	    }
	}
    }
