pipeline{
    agent any
    parameters{
        string(defaultValue: "i-", description: "Instance Id", name: "Instance")
        choice(choices: ['Start', 'Stop', 'Reboot'], description: 'state', name: 'State')
    
    }
    stages{
        stage('one'){
            steps{
                script{
                    if ($"params.State" == "Start")
                    then
                    //aws ec2 start-instances --instance-ids $Instance --region us-east-2
                    echo Instance $InstanceID Started
                    elif ($"params.State" == "Stop")
                    then
                    //aws ec2 stop-instances --instance-ids $Instance --region us-east-2
                    echo Instance $InstanceID Stopped
                    elif ($"params.State" == "Reboot")
                    then
                    //aws ec2 reboot-instances --instance-ids $Instance --region us-east-2
                    echo Instance $InstanceID Restarted
                     fi

                }
            }
        }

    }


}
