properties([
  [
    $class: 'DatadogJobProperty',
    enableProperty: true,
    tagProperties: "commit=\$GIT_COMMIT"
  ]
])

pipeline { 
    agent any 
    stages {
        stage('Test') {
            steps {
                sh 'echo $GIT_COMMIT'
                sh 'sleep 20'
            }
        }
    }
}
