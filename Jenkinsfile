pipeline {
	agent any
	stages {
		stage('Lint HTML') {
			steps {
				sh 'tidy -q -e *.html'
			}
		}
	}
	agent { dockerfile true }
    	stages {
        	stage('Test') {
            		steps {
                		sh 'node --version'
                		sh 'svn --version'
            		}
        	}
    	}
}
