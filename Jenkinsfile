pipeline {
  agent any

environment {
	DB_PASSOWRD = credentials('DB_PASSWORD')
}
  stages {    
    stage('build') {
	steps {
	  sh 'docker-compose build'
	}	      
    }
    stage('run') {
      steps {
        sh 'docker-compose build up -d' 
      }
    }
  }
}
