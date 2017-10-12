node {
    

   
    stage 'promotion'
        def userinput = input(
         id: 'getinput', message: 'Deployment type : Canary or 100% switch', parameters: [
         [$class: 'ChoiceParameterDefinition', name : 'User Input' , choices: 'Choice 1\nChoice 2\nChoice 3' , description : 'Select one']
        ])
    echo ("Choice: " + ${userinput})
}
