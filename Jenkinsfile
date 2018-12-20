pipeline {
    agent any
        stages {
                stage('stage 1') {
			userInput = input(id: 'userInput',    
        	        message: 'Choose an environment',    
                  	parameters: [
                    		[$class:               'ChoiceParameterDefinition', choices: "Dev\nQA\nProd", name: 'Env']
                         ]  
			)
                        steps {
                                sh "/bin/bash testscript.sh && ls"
                        }
                }
        }
}

