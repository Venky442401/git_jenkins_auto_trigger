pipeline {
    agent {
        node {
            label 'agent-test'
        }
    }
    
    stages {
        stage("build"){
            steps{
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
    