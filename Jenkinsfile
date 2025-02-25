pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=killich8_devsecops-jenkins-k8s-tf-sast-sonarcloud-repo -Dsonar.organization=illichk -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=07dd82629ac3e6f3c5563cebd43345b1de266ee8'
			}
        } 
  }
}
