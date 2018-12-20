pipeline {
    agent any
        stages {
                stage('stage 1') {
			input 'Continue the pipeline?'
                        steps {
                                sh "/bin/bash testscript.sh && ls"
                        }
                }
        }
}

