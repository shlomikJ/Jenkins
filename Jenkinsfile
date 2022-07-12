pipeline {
	agent any
	stages {
		stage ('clone git project'){
			steps {
			
			echo "job name is: ${env.JOB_BASE_NAME}"
			git branch: 'master', credentialsId: 'a1fba2eb-44ba-4623-a2a8-d2b8d51e1887', url: 'https://github.com/shlomikJ/Jenkins.git'
			sh "cp /var/jenkins-home/workspace/shlomi/${env.JOB_BASE_NAME}/README.md /tmp/ReadCopy.txt"
				
			}
		}
	}
}	
