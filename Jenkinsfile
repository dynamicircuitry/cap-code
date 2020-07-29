pipeline {
	agent any
	stages {
		stage('Lint HTML') {
			steps {
				sh 'tidy -q -e *.html'
			}
		}
        	stage('Docker Build') {
		agent { dockerfile true }
            		steps {
                		sh 'node --version'
                		sh 'svn --version'
            		}
        	}
    	}
}
