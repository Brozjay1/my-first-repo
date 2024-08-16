pipeline{
    agent any
    stages{
        stage("Greet User"){
            steps{
                sh '''
                    echo "Hello Brozjay\n
                    I believe you want to build an image, do that below"
                '''
            }
        }
        stage("Build image"){
            steps{
                sh '''
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