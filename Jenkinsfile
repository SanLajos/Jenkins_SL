pipeline {
           agent any
           stages {
                stage("Ping") {
                     steps {
                          sh 'ping  google.hu -c 4'
                     }
                }
                stage("Loop") {
                     steps {
                timeout(time: 1, unit: 'MINUTES') {
                    sh  'echo "Hello World!"'
                     }
                }
                }
           }
      }
	 