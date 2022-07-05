properties([pipelineTriggers([githubPush()])])

pipeline {
    agent any
    stage('checkout') {
      steps {
    sudo checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/eranmekler/webhook.git']]])
    sudo echo 'success!'
      }

    }

}