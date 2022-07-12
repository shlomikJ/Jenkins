pipeline {
	agent any
	
	stage ('clone git project')
		step{
		git 'http://githb.com/my_prod'
		script{
			scp user1@remote:/home/user1/file1.txt user2@remote:/home/user2/file2.txt
			}
		}
	}
}	