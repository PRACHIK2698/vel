pipeline {
			agent {
					label {
								label "Slave-1-JNLP"
								customWorkspace "/mnt/slave-2"
						}
			}
			
			stages {
						stage ("one") {
						
							steps {
									sh "yum install httpd -y"
									
							}
						
						}
						
						stage ("two") {
						
							steps {
									sh " yum install git"
								        sh 'echo "My new path"'
									
							}
						
						}
			}
}
