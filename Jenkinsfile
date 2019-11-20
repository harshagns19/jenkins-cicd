pipeline {
	agent any
	
	stages {
	
		stage('Build'){
			steps {
				
				echo 'stage 1'
				sh 'mvn clean package'
			}
		}
		
		stage('Deploy'){
			steps{
				
				echo 'stage 2'
				sh 'mvn clean package'
	}
	
	}
	
	
}
}