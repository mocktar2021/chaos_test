pipeline {
    agent{label 'FPCMS-EKS-NP-NODE-DIT'}
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
                sh 'echo "${Scenario}"'
            }
        }
    }
}
