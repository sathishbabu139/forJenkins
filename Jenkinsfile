pipeline {
    agent any
  
    stages {
	
      	stage (‘SourceBuild’) {
		steps {
        sh 'sudo scp -i /var/lib/jenkins/workspace/jenkinsEmailSend/*  ubuntu@ip-172-31-35-212:/var/www/html/'
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
