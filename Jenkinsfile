pipeline {
    agent any

    parameters {
         gitParameter name: 'BRANCH_TAG', 
                     type: 'PT_BRANCH_TAG',
                     branchFilter: 'origin/(.*)',
                     defaultValue: 'master',
                     selectedValue: 'DEFAULT',
                     sortMode: 'DESCENDING_SMART',
					 description: 'Select your branch or tag.'
		choice(name: 'SonarQube', choices: ['False','True'],description: '')	
    }
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
           stage('Test') {
            steps {
                script{
                    sh 'go test -v -cover ./...'
                }
            }
        }
        stage('Build') {
            steps {
                script{
                    sh 'go build -o cs ./main.go'
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
