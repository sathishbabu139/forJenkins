pipeline {
    agent any
  
    stages {
	try {
      	stage (‘SourceBuild’) {
		sudo cp -R /var/lib/jenkins/workspace/jenkinsEmailSend/* /var/www/html/
		
        echo "Jenkins build is working"
	 
}
	 
}
} catch (Exception ex) {
        currentBuild.result = 'Failed'
    }


        stage('Build') {
            steps {
                mail bcc: '', body: 'This is a message from Jenkins ;The build is Success...!', cc: '', from: '', replyTo: '', subject: 'testing jenkins', to: 'sathishbabu.ganeshan@neshinc.com'
            }
        }
        
    }
}
