pipeline {
    agent any

    stages {
        stage('Example') { 
            steps {
                            echo 'ssssin!'
            }
        }
        stage('Example2') {
            steps {
                            echo 'ssssin2!'
            }
        }
          stage('Clone Code From Github') {
            steps {
                script{
                    sh 'go env'
                }
            }
        }
    }
    post {
        always {
            echo 'I will always say H111ello again!'
        }
}
}
