pipeline {
					
					agent any
					
					tools {
						maven "Maven_Home"
					}
					stages {
						stage('Stage 1 - Checkout Code') {
							steps {
								//Get the code form GITHUB							
                                git 'https://github.com/ajautomation/PassParametersRunTimeViaMVN'
							}
						}
						stage('Stage 2 - Compile Code') {
							steps {
								//cmd to compile the code							
                                sh "mvn compile"
                                //sh "mvn compile"
							}
						}
						stage('Stage 3 - Run Unit Tests') {
							steps {
								//cmd to run tests							
                                sh "mvn test"
							}
						}
						stage('Stage 4 -Create build') {
							steps {
								//cmd to create the build of project							
                                sh "mvn testpackage"
							}
						}
	
					}
					
					}
				
					
				}
