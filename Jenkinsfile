pipeline {
    agent any
    stages {
        stage('One') {
                steps {
                        echo 'Hi, this is Siddhard from Chennai'
			
                }
        }
	    stage('Two'){
		    
		steps {
			echo 'You are in second stage of declarative pipeline'
        }
	    }
        stage('Three') {
                when {
                        not {
                                branch "master"
                        }
                }
                steps {
			echo "Hello"
                        }
        }
        stage('Four') {
                parallel {
                        stage('Unit Test') {
                                steps{
                                        echo "Running the unit test..."
                                }
                        }
 
			}
	     }
        }
    }

