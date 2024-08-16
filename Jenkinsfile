pipeline{
    agent any
    stages{
        stage("Greet User"){
            steps{
                sh '''
                    cd /home/hp
                    echo "Hello Brozjay
                    \nI believe you want to build an image, do that below" > jenkins.txt
                '''
            }
        }
        stage("Build image"){
            steps{
                sh '''
                        cd /home/hp/my-first-repo
                        sudo docker build -t testimage:1
                        echo "Building image please wait loading ----------> completed"
                   '''
            }
    }
    stage("check docker images"){
        steps{
            sh 'sudo docker images'
        }
    }
}
}