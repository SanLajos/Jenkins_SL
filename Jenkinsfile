pipeline {
           agent any
           stages {
                stage("Ping") {
                     steps {
                          ping  google.hu -c 4
                     }
                }
                stage("Loop") {
                     steps {
                timeout(time: 1, unit: 'MINUTES') {
                    sh  'for i in {1..5}
                        do
                            echo "Hello World!"
                            sleep 1
                        done'
                     }
                }
                }
           }
      }
	 