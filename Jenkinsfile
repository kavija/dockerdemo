pipeline{
	agent any
	stages{
		stage('Compile'){
			steps{
				echo "Compile the project - 1"
				echo "Compile the project - 2"
			}
		}
		stage('Build'){
			steps{
				echo "Build the project"
				bat "mvn clean install"
				
				bat "docker build -t kavija/hellodocker:latest ."
			}
		}
		stage('Test'){
			steps{
				echo "Test the project"
			}
		}
		stage('Deploy'){
			steps{
				echo "Deploy the project"
			}
		}
	}
}
