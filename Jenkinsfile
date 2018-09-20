pipeline {
  agent { label "mac" }

  parameters {
		choice(name: 'test_type', choices: 'ui\nios.wdio-mobile', description: 'Type?')
    //Mobile
    choice(name: 'mobileOs', choices: 'android\nios', description: 'Which mobile os (only applicable for mobile suite)')
		choice(name: 'suite', choices: 'acceptance\nsmoke\nregression', description: 'Which suite?')
		string(name: 'subsuite', defaultValue: '', description: 'Subsuite search (will run all tests that have the search value in their filename)')

    //System
    string(defaultValue: '10.187.68.82', description: 'Cadbuild vpn?', name: 'vpn')
    }

  stages {
    stage('Chosen Input') {
      steps {
      	echo "you choose type: ${params.test_type}, suite: ${params.suite}, Sub suite: ${params.subsuite}, ENV: ${params.mobileOs}"
      }
    }

    stage('Mobile Test') {
      steps {
          sh "`which npm` install --strict-ssl false --loglevel warn"
      }
    }
  }

}

