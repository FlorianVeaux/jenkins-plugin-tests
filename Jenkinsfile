properties([
  [
    $class: 'DatadogJobProperty',
    enableProperty: true,
    tagProperties: "time_tag=\$time"
  ]
])

pipeline { 
    agent any 
    stages {
        stage('Test') {
            steps {
                sh 'sleep $time'
            }
        }
    }
}
