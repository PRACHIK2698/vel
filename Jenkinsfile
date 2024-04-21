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
									service start httpd
                                                                        cd /var/www/html/
                                                                        rm -rf *
                                                                        echo "Running Jenking Pipeline using SCM">>/var/www/html/index.html
                                                                        chmod -R 777 /var/www/html/
                                                                        echo "Build job successfually :)"
									
							}
						
						}
			}
}
