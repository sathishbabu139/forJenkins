pipeline {
    agent any
  
    stages {
	
      	stage (‘SourceBuild’) {
		steps {
        sh 'sudo cp -i /var/lib/jenkins/workspace/jenkinsEmailSend/*  /var/www/html/firstBuild'
     echo "${currentBuildcurrentResult} has result success"
		}
}
        stage('EmailNotification') {
            steps {
		    script{
	def check = "${currentBuild.currentResult}"
		    if(check !='SUCCESS'){
		
 mail bcc: '', body: 'This is a message from Jenkins ;The build is Success...!', cc: '', from: '', replyTo: '', subject: 'testing jenkins', to: 'sathishbabu.ganeshan@neshinc.com'
		    }
		    }				      
	    }
        }
        
    }
}

