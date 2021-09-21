pipeline { 
    agent any 
        stages { 
            stage ('Build') { 
                steps { 
                    echo "Running build phase"
					buld.bat
					archiveArtifacts artifacts : 'a.exe' , fingerprint: true
                }
            }
			stage ('Test') { 
                steps { 
                    echo "Running Test phase"
					run.bat
                }
            }
        }
    }
