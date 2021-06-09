pipeline{
    agent any
    stages{
        stage('stage1'){
            steps{
                script{
                    if ( "$State" == "Start" )
                    then
                    aws ec2 start-instances --instance-ids $Instance --region us-east-2
                    echo Instance $InstanceID Started
                    elif ( "$State" == "Stop" )
                    then
                    aws ec2 stop-instances --instance-ids $Instance --region us-east-2
                    echo Instance $InstanceID Stopped
                    elif ( "$State" == "Reboot" )
                    then
                    aws ec2 reboot-instances --instance-ids $Instance --region us-east-2
                    echo Instance $InstanceID Restarted
                     fi

                }
            }
        }

    }


}
