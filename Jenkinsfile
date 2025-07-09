pipeline{
    agent any
    stages{
        stage("test"){
            steps{
                script{
                    echo "Testing the application"
                    echo "Excuting pipeline for branch ${BRANCH_NAME}"

                }
            }
        }
        stage("build"){
            when{
                expression{ BRANCH_NAME == 'master' }
            }
            steps{
                script{
                    echo "Building the application"
                    echo "Excuting pipeline for branch ${BRANCH_NAME}"
                }
            }
        }
        stage("deploy"){
            when{
                expression{ BRANCH_NAME == 'master' }
            }
            steps{
                script{
                    echo "Deploying the application"
                    echo "Excuting pipeline for branch ${BRANCH_NAME}"
                }
            }
        } 
    }
}
