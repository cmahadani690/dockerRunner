pipeline{
	agent any
	stages{
		stage("Run Tests"){
			steps{
				sh "docker-compose up -d"
			}
		}
		stage("Bring doker down"){
			steps{
				sh "docker-compose down"
			}
		}
	}
}
