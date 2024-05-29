/* Requires the Docker Pipeline plugin */
pipeline {
    agent { 
    	docker 
    		{
     			image 'python:3.12.1-alpine3.19' 
     			args '-v /c/ProgramData/Jenkins/.jenkins/workspace/MyPipeLine_main:/workspace'
     		}  
     }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
    }
}