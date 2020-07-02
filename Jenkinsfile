pipeline { 
    agent any
    options {
        datadog(tags: ['hello:florian', "branch_name:$BRANCH_NAME"])
    }
    stages {
        stage('Test') {
            steps {
                sh 'echo $BRANCH_NAME'
                sh 'sleep 10'
            }
        }
    }
}
