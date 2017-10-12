node {
    

 stage 'promotion'

        def userInput = input(
        id: 'userInput', message: 'input parameters', parameters: [
            [
                $class: 'ChoiceParameterDefinition',
                name: 'ami',
                choices: '1\n2\n3',
                description: 'AMI',
            ],
        ]
    )

    echo ("Selected AMI :: "+userInput)



}
