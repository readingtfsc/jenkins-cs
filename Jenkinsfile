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
        stage('print go-env') {
            steps {
                script{
                    sh 'go env'
                }
            }
        }
        stage('Build') {
            steps {
                script{
                    sh 'go build -o cs mian.go'
                }
            }
        }
          stage('Exec') {
            steps {
                script{
                    sh './cs'
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
