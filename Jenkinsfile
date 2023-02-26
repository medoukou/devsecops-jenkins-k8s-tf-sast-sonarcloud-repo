pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecbuggywebapp -Dsonar.organization=asecbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=6bd8691393dd98bd8c99be27117e0854c19d98e0'
			}
        } 
  }
}
