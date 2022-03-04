pipeline {
			agent none
			stages {
				stage('Build') {
        agent { label :node1 }
					steps {
                  sh 'sleep 5; echo "This is a Build stage"'
					
					}
				}
				stage('Test'){
        agent { label : node2 }
					steps {
					        sh '''
                         sleep 5
                         echo "This is a Test stage"
                         '''
                  
					}
				}
				stage('Deploy'){
        agent { label : node3 }
					steps {
                 sh '''
                    sleep 5
                    echo "This is a Deploy stage"
                 '''   
					
					}
				}
				stage('My-stage'){
        agent { label : node1 }
					steps {
                sh '''
                      sleep 5
                      echo "This id my-stage"
                    '''  
					
					}
				}	
			}
		}
