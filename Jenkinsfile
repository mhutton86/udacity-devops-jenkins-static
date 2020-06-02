pipeline {
	agent any
	options {
		withAWS(credentials:'aws-static',region:'us-west-2')
	}
	stages {
		stage('Upload to AWS') {
			steps {
				s3Upload(path:'./', bucket:'udacity-devops-jenkins-static')
			}
		}
	}
}
