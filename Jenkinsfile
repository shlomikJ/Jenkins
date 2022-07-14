pipeline {
	environment {
        destDir = "/tmp/jenkins/"
        
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
				parameters([
				string(
                                defaultValue: '/var/jenkins_home/', 
                                name: 'STR', 
                                trim: true
                            )
			]
		)
				echo "str"
				echo "current dir: $pwd"
				fileOperations([folderCreateOperation('/tmp/jenkins/')])
				sh 'ls -l'
			echo "job name is: ${env.JOB_BASE_NAME}"
			git branch: 'master', credentialsId: 'a1fba2eb-44ba-4623-a2a8-d2b8d51e1887', url: 'https://github.com/shlomikJ/Jenkins.git'
				sh "cp /var/jenkins_home/workspace/shlomi/${env.JOB_BASE_NAME}/README.md ${env.destdir}/ReadMeCopy.md"
				
			}
		}
	}
}	
