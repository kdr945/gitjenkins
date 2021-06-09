pipeline{
    agent any
//     parameters{
//         string(defaultValue: "i-", description: "Instance Id", name: "Instance")
//         choice(choices: ['Start', 'Stop', 'Reboot'], description: 'state', name: 'State')
    
//     }
    stages{
        stage('ne'){
            steps{
                
                    
                   sh if [ "$State" == "Start" ]
                   sh then
                   sh aws ec2 start-instances --instance-ids $Instance --region us-east-2
                   sh echo Instance $InstanceID Started
                   sh elif [ "$State" == "Stop" ]
                   sh then
                   sh aws ec2 stop-instances --instance-ids $Instance --region us-east-2
                   sh echo Instance $InstanceID Stopped
                   sh elif [ "$State" == "Reboot" ]
                   sh then
                   sh aws ec2 reboot-instances --instance-ids $Instance --region us-east-2
                   sh echo Instance $InstanceID Restarted
                   sh fi

                

                
            }
        }

    }


}
