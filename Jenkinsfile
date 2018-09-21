pipeline {
  agent { label "mac" }
  stages {
    stage('Mobile Test') {
      steps {
          sh "hostname; npm --version; /usr/local/bin/npm install --strict-ssl false --loglevel warn"
      }
    }
  }

}

