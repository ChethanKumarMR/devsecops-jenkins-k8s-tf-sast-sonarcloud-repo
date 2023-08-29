pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=chethanbuggywebapp -Dsonar.organization=chethanbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=566187b8cd08adb09663d7865a5790f856110203'
			}
        } 
  }
}
