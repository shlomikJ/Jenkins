pipeline {
	agent any
	
	stage ('clone git project')
		step{
		git 'https://github.com/shlomikJ/Jenkins/README.md'
		script{
			cp /var/jenkins-homw/workspace/README.md /tmp/ReadCopy.txt
			}
		}
	}
}	
