#!groovy

pipeline {

	agent none

  stages {

  	stage('Maven Install') {

    	agent {

      	docker {

        	image 'maven:sapmachine'

        }

      }

      steps {

      	sh 'mvn clean install'

      }

    }

  }

}
