pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecbuyggywebap -Dsonar.organization=asecbuyggywebap -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=058b7fead465401a025c60601da3696ee2d01895'
			}
        } 
  }
}
