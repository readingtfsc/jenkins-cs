
pipeline {
    // agent指定了流水线的执行节点。
    agent any
    // stages是流水线的整个运行阶段，包含一个或多个 stage , 建议 stages 至少包含一个 stage。
    stages{
         stage('TestCover') {
                steps {
                    echo 'Hello World'
                }
            }
    }

    post {
        always {
            echo 'I will always say Hello again!'
        }
    }

}
