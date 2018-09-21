pipeline {
  agent { label "mac" }
  stages {
    stage('Mobile Test') {
      steps {
          sh "hostname; id; /usr/local/bin/npm install --strict-ssl false --loglevel warn"
      }
    }
  }

}

