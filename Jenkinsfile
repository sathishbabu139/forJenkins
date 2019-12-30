pipeline {
    agent any
  
    stages {
	try {
      	stage (‘SourceBuild’) {
		steps {
        sh 'sudo cp -i /var/lib/jenkins/workspace/jenkinsEmailSend/*  /var/www/html/firstBuild'
        echo "Jenkins build is working"	 
		}
}
	}
	    catch(Exception err){
            currentBuild.result = 'FAILURE'
	    }
        stage('EmailNotification') {
            steps {
		script {
			if(currentBuild.result = 'FAILURE'){	
          mail bcc: '', body: 'This is a message from Jenkins ;The build is Success...!', cc: '', from: '', replyTo: '', subject: 'testing jenkins', to: 'sathishbabu.ganeshan@neshinc.com'
			}
			}	      
	    }
        }
        
    }
}
