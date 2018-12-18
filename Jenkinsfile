defaultBuilderNode(slackChannel: 'jenkins') {
  stage('Checkout') {
    checkout scm
  }
  stage('Build & deploy') {
    container('builder') {
        mvn "deploy"
    }
  }
}