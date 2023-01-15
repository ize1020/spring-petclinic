#!groovy

pipeline {

	agent none

  stages {

  	stage('Maven Install') {

    	agent {

      	docker {

        	image 'maven:3.5.0'
                args '-v $HOME:/home/jenkins_home'

        }

      }

      steps {

      	sh 'mvn clean install'

      }

    }

  }

}
