pipeline { 
    agent any 
        stages { 
            stage ('Build') { 
                steps { 
                    echo "Running build phase2"
		    buld.bat
	            archiveArtifacts artifacts : 'a.exe' , fingerprint: true
                }
            }
	    stage ('Test') { 
                steps { 
                    echo "Running Test phase2"
		    run.bat
                }
            }
        }
    }
