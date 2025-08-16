pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbugswebapp -Dsonar.organization=asgbugswebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=6079869fd9dbdc691f3fe498946ead4973a69186'
			}
        } 
  }
}
