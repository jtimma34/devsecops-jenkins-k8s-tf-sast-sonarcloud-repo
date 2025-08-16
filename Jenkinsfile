pipeline {
  agent any
  tools { 
        maven 'Maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggynginx -Dsonar.organization=asgbuggynginx -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=058b7fead465401a025c60601da3696ee2d01895'
			}
        } 
  }
}
