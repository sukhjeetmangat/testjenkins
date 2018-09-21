pipeline {
  agent { label "mac" }
  node {
    env.NODEJS_HOME = "${tool 'Node 6.x'}"
    env.PATH="${env.NODEJS_HOME}/bin:${env.PATH}"
    sh 'npm --version'
}
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

