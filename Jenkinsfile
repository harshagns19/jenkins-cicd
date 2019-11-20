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
				withCredentials([[$class				:'UsernamePasswordMultiBinding',
								   credentialsId		:'PCF_LOGIN',
								   usernameVariable		:'USERNAME',
								   passwordVariable		:'PASSWORD']]){
								   
									  bat 'cf login -a http://api.run.pivotal.io -u $USERNAME -p $PASSWORD'
								
								   }
	}
	
	}
	
	
}
}