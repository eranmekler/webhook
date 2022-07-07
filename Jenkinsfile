properties([pipelineTriggers([githubPush()])])

pipeline {
    agent any
    stage('checkout') {
      steps {
        checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/eranmekler/webhook.git']]])
        echo 'success!'
      }

    }

}