pipeline{
	agent any
	stages{
		stage("Start Grid"){
			steps{
				sh "docker-compose up -d hub chrome firefox"
			}
		}
		stage("Run Tests"){
			steps{
				sh "docker-compose up search-module book-flight-module"
			}
		}
		stage("Bring doker down"){
			steps{
				sh "docker-compose down"
			}
		}
	}
}
