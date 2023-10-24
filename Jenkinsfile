pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecopswebapp-vinay -Dsonar.organization=devsecopswebapp-vinay -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=0a1a1493799eb281d0183603849b6fbeafd89990'
			}
        } 
  }
}
