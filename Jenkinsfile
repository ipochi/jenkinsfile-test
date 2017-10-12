node {
    

    def userInput = "Blue-Green"

    timeout(time: 15, unit: 'SECONDS') {

        userInput = input(
            id: 'userInput', message: 'input parameters', parameters: [
                [
                    $class: 'ChoiceParameterDefinition',
                    name: 'ami',
                    choices: 'Canary\nBlue-Green',
                    description: 'Select one : Default is blue-green',
                ],
            ]
        )
    }

    stage('Deploy Application') {

    
        if(userInput == 'Canary') {

            echo "Inside canary"

        } else if(userInput == 'Blue-green') {

            echo "Inside blue green"
        }


    }

    stage('Deleting old deployments') {
        
        if(userInput == 'Blue-green') {
            echo "deleting blue-green"
        }      
      
    }
}
