pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=hele-project -Dsonar.organization=HALE -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=cea272d0824bcb57fd0d5f9a461e4461bdf4e425'
			}
        } 
  }
}
