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
        stage('aaaaaa Chaos automation') {
            steps {
		    script {
                sh echo "$Scenario"
		    }
	    }
	}
    }
}
