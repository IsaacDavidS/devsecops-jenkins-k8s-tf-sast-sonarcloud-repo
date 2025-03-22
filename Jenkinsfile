pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp9 -Dsonar.organization=javaprojectaws -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=625b193ca4bf7c4a6f3b1303c14dfdb5e1a13c01'
			}
        } 
  }
}
