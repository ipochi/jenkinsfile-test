node {
    

  parameters {
        choice(
            // choices are a string of newline separated values
            // https://issues.jenkins-ci.org/browse/JENKINS-41180
            choices: 'greeting\nsilence',
            description: '',
            name: 'REQUESTED_ACTION')
    }



    echo params.REQUESTED_ACTION
  /*  stage 'promotion'
        def userinput = input(
         id: 'getinput', message: 'Deployment type : Canary or 100% switch', parameters: [
         [$class: 'ChoiceParameterDefinition', name : 'DEPLOY_TYPE', choices: 'Choice 1\nChoice 2\nChoice 3' , description : 'Select one']
        ])
    echo ("Choice: " + ${userinput})

*/


}
