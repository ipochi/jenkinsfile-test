node {
    

   
    stage 'promotion'
        def userInput = input(
         id: 'userInput', message: 'Deployment type : Canary or 100% switch', parameters: [
         [$class: 'ChoiceParameterDefinition', choices: 'Choice 1\nChoice 2\nChoice 3']
        ])
    echo ("Choice: "+userInput)
}
