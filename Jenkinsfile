node{
  stages {
stage('EmailNotification'){
emailext body: 'This is a Test Email from jenkins build...!', subject: 'TestEmail', to: 'sathishbabu.ganeshan@neshinc.com'
}
stage('Deploy') {
            steps {
                echo 'Deploying'
            }
        }
	}
}	
