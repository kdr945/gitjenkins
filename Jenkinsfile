pipeline{
    agent any
//     parameters{
//         string(defaultValue: "i-", description: "Instance Id", name: "Instance")
//         choice(choices: ['Start', 'Stop', 'Reboot'], description: 'state', name: 'State')
    
//     }
    stages{
        stage('ne'){
            steps{
                script{
                    if("$State"=="Start"){
                        echo 'yes'
                    }else if("$State"=="Stop"){
                        echo 'no'
                    }else if("$State"=="Reboot"){
                        echo 're'
                    }
                }                
              
                
                                  
            }
        }

    }


}
