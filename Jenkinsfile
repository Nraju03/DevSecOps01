pipeline {
  agent any
  tools { 
        maven 'Maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp548_asgbuggywebapp -Dsonar.organization=asgbuggywebapp548 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=7297ddf853c9f4ec9cae08e4db4d8921cb0ae50e'
			}
    }

   }
}
