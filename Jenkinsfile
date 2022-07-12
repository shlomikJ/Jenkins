pipeline {
	agent any
	stages {
		stage ('clone git project'){
			steps {
			dir = env.JOB_BASE_NAME
				echo 'job name is: ${dir}'
			git branch: '*/master', credentialsId: 'a1fba2eb-44ba-4623-a2a8-d2b8d51e1887', url: 'https://github.com/shlomikJ/Jenkins.git'
			sh 'cp /var/jenkins-homw/workspace/shlomi/dir/README.md /tmp/ReadCopy.txt'
				
			}
		}
	}
}	
