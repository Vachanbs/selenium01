pipeline{
	agent any
	tools{
		maven 'Maven'
	}
	stages{
		stage('checkout'){
		steps{
			git branch : 'main' , url : 'https://github.com/Vachanbs/Selenium01.git' 
		}
		}
		stage('build'){
		steps{
			sh 'mvn clean install'
		}}
		stage('test'){
		steps{
			sh 'mvn test'
		}}
		
	}
	post{
		success{
			echo "sucess Bro"
		}
		failure{
			echo "Failure Bro"
		}
	}
	}
