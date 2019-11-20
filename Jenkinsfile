pipeline {
	agent any
	
	stages {
	
		stage('Build'){
			steps {
				
				echo 'stage 1'
				bat 'mvn clean package'
			}
		}
		
		stage('Deploy'){
			steps{
				
				echo 'stage 2'
				bat 'mvn clean package'
	}
	
	}
	
	
}
}