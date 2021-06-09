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
                        aws ec2 start-instances --instance-ids $Instance --region us-east-2
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
