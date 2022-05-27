pipeline {
    agent any

    stages {
        stage('Example') {
        
           
            steps {
                go env
            }
        }
         stage('Example2') {
        
           
            steps {
                go test -v -cover ./...
            }
        }
           stage('Example3') {
        
           
            steps {
                go build -o cs mian.go
            }
        }
    }
    post {
        always {
            echo 'I will always say H111ello again!'
        }
}
}
