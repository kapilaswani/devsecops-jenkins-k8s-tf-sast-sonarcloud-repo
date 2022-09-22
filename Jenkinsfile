pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=aws-buggy-webapp -Dsonar.organization=aws-buggy-webapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=42e4a93f9f55b3bc9463db789205c7c614ae7e67'
			}
        } 
  }
}
