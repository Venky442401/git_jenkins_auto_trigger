pipeline {
    agent {
        node {
            label 'agent-test'
        }
    }
    environment {
        USER_NAME = "venky"
    }
    options {
        timeout(time: 1, unit: 'SECONDS')

    }
    stages {
        stage("build"){
            steps{
                echo "user name ${USER_NAME}"
                echo "build trigger automatically code pushed "
            }
        }
        stage("Teting_something"){
            steps{
                echo "Testing is running"
                echo "Testing is after push"
            }
        }
    }
    post{
           always {
                echo "run always "
            }
            success {
                echo "job successs"
            }
            failure {
                echo "jon failed"
            }
    }
        
}
    