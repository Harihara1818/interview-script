pipeline {
  agent any
  options {
    buildDiscarder(logRotator(numToKeepStr: '2'))
  }
    stages{
      stage('stage-1'){
         steps{
	   echo "hey"
         }
      }
      stage('build-log-lock') {
        steps{
	  script{		      
	    currentBuild.keepLog = true
	  }
	}
      }
    }
}
