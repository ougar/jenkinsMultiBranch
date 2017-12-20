node {
  stage('Checkout') {
    checkout scm
  }
  stage('Test') {
    sh "echo Test"
    sh "ls -la"
  }
  stage('Build') {
    sh "docker build -t rtest1 ."
  }
  stage('Run') {
    sh "echo Run"
    sh "docker run rtest1"
  }
}
