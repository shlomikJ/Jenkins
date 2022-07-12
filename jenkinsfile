pipeline {
	agent any
	
	stage ('clone git project')
		step{
		git 'https://github.com/shlomikJ/Jenkins/README.md'
		script{
			scp shlomi@192.168.50.155:'/var/jenkins_home/workspace/copy ReadMe git/README.md' 274068@192.168.50.1:D:\Git\Demo\file2.txt
			}
		}
	}
}	
