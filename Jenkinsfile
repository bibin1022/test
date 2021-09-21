pipeline { 
    agent any 
        stages { 
            stage ('Build') { 
                steps { 
                    echo "Running build phase2"
		    bat "build.bat"
		    archiveArtifacts artifacts : 'a.exe' , fingerprint: true
                }
            }
	    stage ('Test') { 
                steps { 
                    echo "Running Test phase2"
		    bat "run.bat"
                }
            }
        }
    }
