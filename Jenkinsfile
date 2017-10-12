node {
    

   
    stage 'promotion'
        def userInput = input(
         id: 'userInput', message: 'Deployment type : Canary or 100% switch', parameters: [
         [$class: 'ChoiceParameterDefinition', choices: 'uat , dev , prod']
        ])
    echo ("Env: "+userInput['env'])
    echo ("Target: "+userInput['target'])
}
