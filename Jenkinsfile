pipeline {
    agent any
  
    stages {
	
      	stage (‘SourceBuild’) {
		steps {
        sh 'sudo cp -i /var/lib/jenkins/workspace/jenkinsEmailSend/*  /var/www/html/firstBuild'
        echo "Jenkins build is working"	 
		}
}
	
        stage('Build') {
            steps {
                mail bcc: '', body: 'This is a message from Jenkins ;The build is Success...!', cc: '', from: '', replyTo: '', subject: 'testing jenkins', to: 'sathishbabu.ganeshan@neshinc.com'
            }
        }
        
    }
}
