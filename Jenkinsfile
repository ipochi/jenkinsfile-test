node {
    

    def userInput = "Blue-Green"

    try {
        timeout(time: 20, unit: 'SECONDS') {

            userInput = input(
                id: 'userInput', message: 'input parameters', parameters: [
                    [
                        $class: 'ChoiceParameterDefinition',
                        name: 'ami',
                        choices: 'Blue-Green\nCanary',
                        description: 'Select one : Default is blue-green',
                    ],
                ]
            )
        }
    } catch(err) { // timeout reached or input false
        def user = err.getCauses()[0].getUser()
        if('SYSTEM' == user.toString()) { // SYSTEM means timeout.
            userInput = "Blue-Green";
    } else {
        echo "Aborted by: [${user}]"
    }
}
echo "USER INPUT --- " + userInput
    
    stage('Deploy Application') {

    
        if(userInput == 'Canary') {

            echo "Inside canary"

        } else if(userInput == 'Blue-Green') {

            echo "Inside blue green"
        }


    }

    stage('Deleting old deployments') {
        
        if(userInput == 'Blue-Green') {
            echo "deleting blue-green"
        }      
      
    }
}
