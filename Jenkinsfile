pipeline {
	agent any
	stages {
		stage ('clone git project'){
			steps {
			git 'https://github.com/shlomikJ/Jenkins/README.md'
			script{
				cp /var/jenkins-homw/workspace/README.md /tmp/ReadCopy.txt
				}
			}
		}
	}
}	
