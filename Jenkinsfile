pipeline {
    agent any
    stages {
        stage('# Packaging') {
            steps {
              sh "mvn clean package"
            }
        }  
	    hh
		stage('Step 12 archive artifacts') {
            steps {
             archiveArtifacts artifacts: '**/*.war', fingerprint: true
            }
        }
}
}
