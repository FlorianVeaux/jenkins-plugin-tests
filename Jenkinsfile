properties([
  [
    $class: 'DatadogJobProperty',
    enableProperty: true,
    tagProperties: 'commit=$GIT_COMMIT\ntest=$TEST_TAG'
  ]
])

pipeline { 
    agent any 
    environment {
        GIT_COMMIT = "$GIT_COMMIT"
        TEST_TAG   = "hello"
    }
    stages {
        stage('Test') {
            steps {
                sh 'echo $GIT_COMMIT'
                sh 'echo $TEST_TAG'
                sh 'sleep 20'
            }
        }
    }
}
