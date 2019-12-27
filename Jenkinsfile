pipeline {
    agent any
    options {
        skipStagesAfterUnstable()
    }
    stages {
	stage('EmailNotification'){
	emailext body: 'This is a Test Email from jenkins build...!', subject: 'TestEmail', to: 'sathishbabu.ganeshan@neshinc.com'

	}
 	stage('Build') {
            steps {
                echo 'Building'
            }
        }
    
        stage('Test') {
            steps {
                echo 'Testing'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying'
            }
        }
}
}
