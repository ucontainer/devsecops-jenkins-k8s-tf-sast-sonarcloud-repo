pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=ucontainerbuggy -Dsonar.organization=ucontainerorg -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=24ef0b97818a59b68c8cd8bea69c1f7567de57f6'
			}
        } 
  }
}
