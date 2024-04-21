pipeline {
  agent any
  tools { 
        maven 'Maven_3_9_6'
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=
asecuritywebbuggyapp-pro -Dsonar.organization=asecuritywebbuggyapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=a0296d3defe76c6557b7c69be94160755a44a531'
			}
        } 
  }
}
