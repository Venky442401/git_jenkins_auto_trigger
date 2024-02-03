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
    