node {
    

   
    stage 'promotion'
        def userInput = input(
         id: 'userInput', message: 'Deployment type : Canary or 100% switch', parameters: [
         [$class: 'ChoiceParameterDefinition', choices: 'canary' , choices:'blue-green']
        ])
    echo ("Choice: "+userInput)
}
