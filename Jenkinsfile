pipeline {
	// agent any
	agent { docker { image 'maven:3.6.8'} }
		stages {
			stage('build'){
				steps{
					sh "mvn --version"
					echo "build"
				}
			}
			stage('test'){
				steps{
					echo "test"
				}
			}
		} 
		post {
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
