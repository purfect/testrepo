pipeline {
    agent any
	userInput = input(id: 'userInput',    
                  message: 'Choose an environment',    
                  parameters: [
                    [$class:               'ChoiceParameterDefinition', choices: "Dev\nQA\nProd", name: 'Env']
                         ]  
)
        stages {
                stage('stage 1') {
                        steps {
                                sh "/bin/bash testscript.sh && ls"
                        }
                }
        }
}

