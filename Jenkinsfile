pipeline {
	environment {
        destDir = "/tmp/jenkins/"
        Str= "/var/jenkins_home/"
    }
	agent any
	stages {
		stage ('clean workspace'){
			steps {
			echo "clean dir"
			step([$class: 'WsCleanup'])
			}
		}
		
		stage ('clone git project'){
			
			steps {
				
				echo "$env.Str"
				echo "current dir: $pwd"
				fileOperations([folderCreateOperation(${env.destDir})])
				sh 'ls -l'
			echo "job name is: ${env.JOB_BASE_NAME}"
			git branch: 'master', credentialsId: 'a1fba2eb-44ba-4623-a2a8-d2b8d51e1887', url: 'https://github.com/shlomikJ/Jenkins.git'
				sh "cp /var/jenkins_home/workspace/shlomi/${env.JOB_BASE_NAME}/README.md ${env.destdir}TEMP/ReadMeCopy.md"
				
			}
		}
	}
}	
