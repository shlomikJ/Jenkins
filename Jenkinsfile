pipeline {
	agent any
	stages {
		stage ('clone git project'){
			steps {
			git branch: '*/master', credentialsId: 'a1fba2eb-44ba-4623-a2a8-d2b8d51e1887', url: 'https://github.com/shlomikJ/Jenkins.git'
			script{
				cp /var/jenkins-homw/workspace/shlomi/{env.JOB_BASE_NAME}/README.md /tmp/ReadCopy.txt
				}
			}
		}
	}
}	
