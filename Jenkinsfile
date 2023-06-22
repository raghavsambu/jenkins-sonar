pipeline {
  agent any
  tools {       
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=jenkinswest_jenkinswest -Dsonar.organization=jenkinswest -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=8934c458cc10e891e2a668114f48f6e017f259ce'
			}
        } 
  }
}
