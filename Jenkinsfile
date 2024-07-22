pipeline {
	agent any
		stages{
			stage('build'){
				steps{
					echo "build"
				}
			}
			stage('test'){
				steps{
					echo "test"
				}
			}
		} post{
			always{
				echo "i execute always"
			}
			success{
				echo "i execute when build is successful"
			}
			failure{
				echo "i execute when build is failed"
			}
		}

}
