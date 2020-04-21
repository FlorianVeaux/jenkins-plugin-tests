properties([
  [
    $class: 'DatadogJobProperty',
    enableProperty: true,
    tagProperties: "branch=\$BRANCH_NAME"
  ]
])

pipeline { 
    agent any 
    stages {
        stage('Test') {
            steps {
                sh 'echo $BRANCH_NAME'
                sh 'sleep '30'
            }
        }
    }
}
