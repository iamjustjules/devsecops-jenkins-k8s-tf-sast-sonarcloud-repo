pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=iamjustjules -Dsonar.organization=iamjustjules -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=20d4809a06afe96cc8d4ebdb0ebaf2de36bfbe26'
			}
        } 
  }
}
