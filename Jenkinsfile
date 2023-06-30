pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecops-learn_asgbuggywebapp -Dsonar.organization=devsecops-learn -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=9dc484e709d858996ce93f109a6442adffd51add'
			}
        } 
  }
}
