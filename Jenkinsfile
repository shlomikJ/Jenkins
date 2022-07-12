pipeline {
	agent any
	stages {
		stage ('clone git project'){
			steps {
			git 'https://github.com/shlomikJ/Jenkins.git'
			script{
				cp /var/jenkins-homw/workspace/shlomi/README.md /tmp/ReadCopy.txt
				}
			}
		}
	}
}	
