pipeline {
    agent any
  
    stages {
	
      	stage (‘SourceBuild’) {
		steps {
        sh 'sudo cp -i /var/lib/jenkins/workspace/jenkinsEmailSend/*  /var/www/html/firstBuild'
        echo "Jenkins build is working"	 
		}
}
	
        stage('EmailNotification') {
            steps {
		    script {
                    FAILED_STAGE=env.STAGE_NAME
                   
                }
          mail bcc: '', body: 'This is a message from Jenkins ;The build is Success...! from stage ${FAILED_STAGE}', cc: '', from: '', replyTo: '', subject: 'testing jenkins', to: 'sathishbabu.ganeshan@neshinc.com'
	  	      
	    }
        }
        
    }
}
