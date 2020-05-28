 script {
            // Define Variable
             def USER_INPUT = input(
                    message: 'Please input you name of service you need to build ^^',
                    parameters: [
                            [$class: 'ChoiceParameterDefinition',
                             choices: ['Bridge','BridgeAdmin','Notification','Store','Solomon'].join('\n'),
                             name: 'input',
                             description: 'Menu - select box option']
                    ])

            echo "The answer is: ${USER_INPUT}"

            if( "${USER_INPUT}" == "Bridge"){
                echo "You chose the Bridge service to deploy, right ?"
                def USER_INPUT2 = input2(
                    message: 'Please input you name of service you need to build ^^',
                    parameters: [
                            [$class: 'ChoiceParameterDefinition',
                             choices: ['yes','no'].join('\n'),
                             name: 'input2',
                             description: 'Menu - select box option']
                    ])
                     if( "${USER_INPUT2}" == "yes"){
                         echo "bridge will deploy in 3 seconds ..."
                         sleep 3
                     } else {
                         echo "You chose NO, so exit"
                     }
            } else {
                //do something else
            }
        }
