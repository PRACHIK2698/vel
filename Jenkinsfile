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
									sh "sudo yum install httpd -y"
									
							}
						
						}
						
						stage ("two") {
						
							steps {
									sh "sudo service httpd start"
									sh "sudo cp -r index.html /var/www/html/"
									sh "sudo chmod -R 777 /var/www/html/"
									
							}
						
						}
			}
}
