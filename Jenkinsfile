pipeline {
  agent { label "mac" }
  tools {
        nodejs 'node 7'
    }
  stages {
    stage('Mobile Test') {
      steps {
          sh "hostname; /usr/local/bin/npm --version; /usr/local/bin/npm install --strict-ssl false --loglevel warn"
      }
    }
  }

}

